```markdown

# Reference: Pine to MQL5 Snippets Library (Full Parity Edition)

This library provides production-ready, high-performance code snippets for every rule, mapping, and trap defined in the [Pine Script to MQL5 Conversion guide](https://github.com/GeoKFX/MQL5_Snippets_and_Skills/blob/main/skills/Pine-Script-to-MQL5-Conversion/SKILL.md). It is designed to ensure 1:1 logical parity between Pine Script v5/v6 and MQL5.

---

## CORE_EXECUTION_STATE

### 1.1 var vs varip (Persistence & Lifecycle Management)

Pine Script handles persistence implicitly. In MQL5, we use `static` variables, but we must explicitly manage the "History Reset" event to prevent stale data from corrupting calculations during symbol/timeframe changes.

```cpp
// [RULE 1.1a] var (Historical Persistence)
// Pattern: Static variable with a hard-reset guard in OnCalculate.
int OnCalculate(...) {
    static double m_highestEver = 0.0;
    
    // CRITICAL: When history is reloaded (prev_calculated == 0), 
    // static variables persist in memory. We MUST manually reset them.
    if(prev_calculated == 0) {
        m_highestEver = -DBL_MAX; // Use minimum double value for 'Highest' logic
    }

    if(high[0] > m_highestEver) m_highestEver = high[0];
    return(rates_total);
}

// [RULE 1.1b] varip (Intrabar Persistence)
// Pattern: Static variable with Manual New Bar Detection for "In-Progress" states.
int OnCalculate(...) {
    static datetime m_lastBarTime = 0;
    static double m_volumeAccumulator = 0; // Cumulative volume within the current bar

    // Detect if the current tick belongs to a new bar
    if(time[0] != m_lastBarTime) {
        m_volumeAccumulator = 0.0; // Reset state for the new candle
        m_lastBarTime = time[0];
    }
    
    // Accumulate data on every tick (equivalent to Pine's varip)
    m_volumeAccumulator += tick_volume[0];
    return(rates_total);
}
```

### 1.2 Incremental Looping (Efficiency & Recursive Integrity)

The `O(N^2)` trap occurs when developers recalculate the entire history on every tick. Following the incremental pattern is vital for low-latency trading.

```cpp
// [RULE 1.2] The Standard Incremental Loop
int OnCalculate(...) {
    // Determine the starting index. 
    // If prev_calculated > 0, we start from the last known calculated bar (-1 to re-check forming bar).
    int start = (prev_calculated > 0) ? prev_calculated - 1 : 0;

    for(int i = start; i < rates_total; i++) {
        // Recursive Integrity: Formulas like EMA rely on the previous bar's value.
        // Recalculating the 'forming' bar (index i) ensures the recursive state 
        // is updated as price moves within the candle.
        buffer[i] = some_recursive_calc(buffer[i-1], close[i]);
    }
    return(rates_total);
}
```

### 1.3 Indexing Direction (Visual Alignment)

MQL5 arrays grow from 0 (oldest) to rates_total-1 (newest). Pine uses `[0]` for newest. `ArraySetAsSeries` bridges this gap.

```cpp
// [RULE 1.3] Forcing Reverse-Chronological Indexing
void SetupBuffers(double &buffer1[], double &buffer2[]) {
    // Sets arrays to 'Series' mode so index 0 = Current Bar
    ArraySetAsSeries(buffer1, true);
    ArraySetAsSeries(buffer2, true);
}
```

---

## DATA_STRUCTURE_MAPPING

### 2.1 User Defined Types (UDTs)

Pine v6 UDTs are best mapped to classes. This enables encapsulation and helper methods that mimic Pine's functional features.

```cpp
// [RULE 2.1] Complex UDT implementation
class CSignalState {
private:
    double m_threshold;
    string m_comment;
public:
    double price;
    bool   is_valid;

    CSignalState(double p, double t, string c) : price(p), m_threshold(t), m_comment(c) {
        is_valid = (price > m_threshold);
    }
    
    // Equivalent to Pine v6 Methods
    void Update(double newPrice) {
        price = newPrice;
        is_valid = (price > m_threshold);
    }
};
```

### 2.2 Advanced Collections (Mapping Performance)

MQL5 lacks native multi-type matrices, so we use standardized collections or flattened arrays.

```cpp
// [RULE 2.2a] Pine Map -> MQL5 HashMap
#include <Generic\HashMap.mqh>
CHashMap<string, double> m_paramMap; // Store key-value pairs for dynamic settings

// [RULE 2.2b] Pine Matrix -> Optimized 1D Wrapper
class CMatrix2D {
private:
    double m_data[];
    int    m_cols;
public:
    CMatrix2D(int rows, int cols) : m_cols(cols) { ArrayResize(m_data, rows * cols); }
    void   Set(int r, int c, double val) { m_data[r * m_cols + c] = val; }
    double Get(int r, int c) { return m_data[r * m_cols + c]; }
};
```

---

## MTF_SECURITY_ALIGNMENT

### 3.1 Non-Repainting Security (The Gold Standard)

Repainting occurs when an indicator uses future data. The `shift + 1` rule is the only way to guarantee parity with Pine’s `lookahead = barmerge.lookahead_off`.

```cpp
// [RULE 3.1] Secure Multi-Timeframe Data Retrieval
double GetClosedHTFValue(string symbol, ENUM_TIMEFRAMES htf_tf, datetime ltf_time) {
    // Find the HTF bar index that contains the LTF timestamp
    int shift = iBarShift(symbol, htf_tf, ltf_time, false);
    
    if(shift == -1) return EMPTY_VALUE;
    
    // We MUST use shift + 1. 
    // Index 'shift' represents the HTF bar that is currently forming relative to LTF.
    // Index 'shift + 1' is the bar that was already CLOSED when the LTF bar started.
    return iClose(symbol, htf_tf, shift + 1);
}
```

### 3.2 Data Synchronization Guard

MQL5 data requests are asynchronous. You must validate the return of `iBarShift` and other data access functions to prevent array out-of-range errors and logic corruption.

```cpp
// [RULE 3.2] Safety Guard for MTF Access
int htf_index = iBarShift(_Symbol, PERIOD_H4, time[i], false);

if(htf_index == -1) {
    // History not loaded or sync error. 
    // In Pine, this returns 'na'. In MQL5, we must skip or use a fallback.
    buffer[i] = EMPTY_VALUE; 
    return; // Or continue in loop
}
```

---

## STRATEGY_EA_PARITY

### 4.1 Execution Gating (Parity Engine)

Pine backtests on bar close. MQL5 live trading happens on every tick. Failing to gate execution leads to "Hyper-trading" and different results.

```cpp
// [RULE 4.1] Synchronized Bar-Close Execution
bool IsNewBar(ENUM_TIMEFRAMES period = PERIOD_CURRENT) {
    static datetime lastTime = 0;
    datetime curTime = iTime(_Symbol, period, 0);
    
    if(curTime != lastTime) {
        lastTime = curTime;
        return true;
    }
    return false;
}

void OnTick() {
    if(!IsNewBar()) return; // Parity: Logic only executes when a new candle opens
    // Trading Logic ...
}
```

### 4.2 ECN-Compatible Orders

ECN brokers often reject orders with SL/TP attached in the initial `OrderSend`.

```cpp
// [RULE 4.2] Robust ECN Execution Pattern
#include <Trade\Trade.mqh>
CTrade trade;

void SafeTradeEntry(double volume, double sl, double tp) {
    // 1. Send the entry order first
    if(trade.Buy(volume, _Symbol)) {
        ulong ticket = trade.ResultOrder();
        // 2. Modify position to set SL/TP only after entry is confirmed
        if(ticket > 0) {
            trade.PositionModify(_Symbol, NormalizeDouble(sl, _Digits), NormalizeDouble(tp, _Digits));
        }
    }
}
```

### 4.3 Pyramiding Logic

MQL5 does not automatically stack positions or limit them like Pine's `pyramiding` parameter. You must manually count and filter current positions.

```cpp
// [RULE 4.3] Manual Pyramiding Check
int CountStrategyPositions(long magic) {
    int count = 0;
    for(int i = PositionsTotal() - 1; i >= 0; i--) {
        ulong ticket = PositionGetTicket(i);
        if(PositionSelectByTicket(ticket)) {
            // Filter by current symbol and your specific Magic Number
            if(PositionGetString(POSITION_SYMBOL) == _Symbol && 
               PositionGetInteger(POSITION_MAGIC) == magic) {
                count++;
            }
        }
    }
    return count;
}

// Usage in Strategy Logic:
if(CountStrategyPositions(MyMagicNumber) < MaxPyramiding) {
    trade.Buy(LotSize);
}
```

---

## SILENT_TRAPS_CHECKLIST

### TRAP_1: Floating Point Drift

```cpp
// Prices MUST be normalized to the symbol's specific digit precision.
// Failure results in 'Invalid Stops' or 'Invalid Price' errors.
double cleanSL = NormalizeDouble(Bid - 50 * _Point, _Digits);
```

### TRAP_2: Recursive Drift (EMA/RMA)

```cpp
// Pine RMA (Relative Moving Average) uses 1/Length alpha.
// Parity requires persistent storage of the previous result.
static double prevRMA = 0;
double alpha = 1.0 / 14.0;
if(prev_calculated == 0) prevRMA = close[0];
double currentRMA = alpha * close[0] + (1.0 - alpha) * prevRMA;
prevRMA = currentRMA;
```

### TRAP_3: Implicit NaN (`na` propagation)

```cpp
// Pine: val = nz(src) -> If src is na, use 0.
// MQL5: Use MathIsValidNumber check to prevent NaN poisoning.
double val = iRSI(_Symbol, _Period, 14, 0);
if(!MathIsValidNumber(val)) val = 0.0; 
```

### TRAP_4: Array Direction Consistency

Mixing indexed series (`ArraySetAsSeries = true`) with forward-indexed arrays in the same mathematical formula is the most common cause of signal inversion and lag.

```cpp
// [TRAP 4] Enforce consistency across all calculation components
void ValidateExecutionModel(double &buffer[], const double &price[]) {
    if(!ArrayGetAsSeries(buffer)) ArraySetAsSeries(buffer, true);
    if(!ArrayGetAsSeries(price))  ArraySetAsSeries(price, true);
    
    // Now both follow Pine's [0] = current logic safely
    buffer[0] = price[0] - price[1]; 
}
```

### TRAP_5: Integer Division (Silent Truncation)

```cpp
// Pine: 5 / 2 = 2.5
// MQL5: 5 / 2 = 2 (Integer result)
double correctVal = (double)5 / 2; // Returns 2.5
```
```
