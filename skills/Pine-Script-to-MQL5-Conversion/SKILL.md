

# [SKILL] Pine Script to MQL5 Conversion

| | |
| :--- | :--- |
| **name** | PineScript-to-MQL5-Architect |
| **description** | Expert system for deterministic conversion of Pine Script v5/v6 to MQL5 with zero-repainting guarantees. |
| **triggers** | Convert, Pine, Pine script, PineScript, TV, Trading view, MQL5 indicator, OnCalculate, indicator buffers, MT5. |
| **allowed-tools** | Google_search, Read, Grep, Edit, Write |

## TABLE OF CONTENTS

1. [CORE_EXECUTION_STATE](#core_execution_state)
2. [DATA_STRUCTURE_MAPPING](#data_structure_mapping)
3. [MTF_SECURITY_ALIGNMENT](#mtf_security_alignment)
4. [STRATEGY_EA_PARITY](#strategy_ea_parity)
5. [SILENT_TRAPS_CHECKLIST](#silent_traps_checklist)
6. [REFERENCE_DOCUMENTATION](#reference_documentation)

---

## CORE_EXECUTION_STATE

This section handles the translation of Pine's vectorized execution into MQL5's event-driven state machine.

* **Rule 1.1 (var/varip):** Replicate persistence using `static` variables. `var` requires a `prev_calculated == 0` guard. `varip` requires manual "New Bar" detection to manage intrabar state.

```cpp
// Rule 1.1 Implementation
static double m_historicalVar; // var equivalent
if(prev_calculated == 0) m_historicalVar = 0.0;

static datetime lastBarTime = 0;
static double m_tickAccumulator = 0; // varip equivalent
if(time[0] != lastBarTime) {
    m_tickAccumulator = 0.0; 
    lastBarTime = time[0];
}
m_tickAccumulator += 1.0;
---

---

## [CORE_EXECUTION_STATE]

This section handles the translation of Pine's vectorized execution into MQL5's event-driven state machine.

* **Rule 1.1 (var/varip):** Replicate persistence using `static` variables. `var` requires a `prev_calculated == 0` guard. `varip` requires manual "New Bar" detection to manage intrabar state.

```cpp
// Rule 1.1 Implementation
static double m_historicalVar; // var equivalent
if(prev_calculated == 0) m_historicalVar = 0.0;

static datetime lastBarTime = 0;
static double m_tickAccumulator = 0; // varip equivalent
if(time[0] != lastBarTime) {
    m_tickAccumulator = 0.0; 
    lastBarTime = time[0];
}
m_tickAccumulator += 1.0;
```

* **Rule 1.2 (Looping):** Implement incremental loops: `int start = (prev_calculated > 0) ? prev_calculated - 1 : 0`. Re-evaluating the current bar is mandatory for recursive integrity.

```cpp
// Rule 1.2 Implementation
int start = (prev_calculated > 0) ? prev_calculated - 1 : 0;
for(int i = start; i < rates_total; i++) {
    // Logic here maintains recursive integrity (EMA/RMA)
}
```

* **Rule 1.3 (Indexing):** Enforce `ArraySetAsSeries(true)` to align MQL5 with Pine’s reverse-chronological indexing `[0]`.

```cpp
// Rule 1.3 Implementation
ArraySetAsSeries(close, true);
ArraySetAsSeries(buffer, true);
```

---

## [DATA_STRUCTURE_MAPPING]

Mapping functional Pine v6 structures to Object-Oriented MQL5.

* **Rule 2.1 (UDTs):** Convert Pine `type` definitions to MQL5 `class` structures. Classes support methods and dynamic memory via `CArrayObj`.

```cpp
// Rule 2.1 Implementation
class CPineUDT {
public:
    double price;
    string label;
    CPineUDT(double p, string l) : price(p), label(l) {}
    double GetOffset(double current) { return MathAbs(price - current); }
};
```

* **Rule 2.2 (Collections):** * Pine Map → `CHashMap<K, V>`.
    * Pine Matrix → Flattened 1D array with `IDX(r, c)` macro access.
    * Pine Array → `CArrayDouble` or native dynamic arrays.

```cpp
// Rule 2.2 Implementation
#include <Generic\HashMap.mqh>
CHashMap<string, double> m_map; // Map

#define MAT_IDX(r, c, cols) ((r) * (cols) + (c)) // Matrix flattening
double m_matrix[]; 
```

---

## [MTF_SECURITY_ALIGNMENT]

Deterministic time alignment for `request.security` without future-leaks.

* **Rule 3.1 (Shift + 1 Rule):** Use `iBarShift` to align LTF time to HTF index. Always access `[shift + 1]` for closed-bar data (lookahead_off parity).

```cpp
// Rule 3.1 Implementation
int htf_shift = iBarShift(sym, tf, ltf_time, false);
double htf_closed_val = iClose(sym, tf, htf_shift + 1); 
```

* **Rule 3.2 (Sync Guard):** Always validate `iBarShift` return values (`!= -1`) before data access to prevent array out-of-range errors.

```cpp
// Rule 3.2 Implementation
if(htf_shift == -1) {
    buffer[i] = EMPTY_VALUE; // Handle missing data sync
    return; 
}
```

---

## [STRATEGY_EA_PARITY]

Ensuring Pine backtest results match MQL5 Live Execution.

* **Rule 4.1 (Execution Gating):** Use an `IsNewBar()` filter in `OnTick()` to mimic Pine's bar-close evaluation model.

```cpp
// Rule 4.1 Implementation
bool IsNewBar() {
    static datetime lastTime = 0;
    datetime curTime = iTime(_Symbol, _Period, 0);
    if(curTime != lastTime) { lastTime = curTime; return true; }
    return false;
}
```

* **Rule 4.2 (ECN Protocol):** Follow the "Open-then-Modify" sequence: `trade.Buy()` -> `ResultOrder()` -> `trade.PositionModify()`.

```cpp
// Rule 4.2 Implementation
if(trade.Buy(0.1, _Symbol)) {
    trade.PositionModify(_Symbol, sl, tp); // ECN compatible
}
```

* **Rule 4.3 (Pyramiding):** Manually track position counts using `PositionsTotal()` filtered by Magic Number and Symbol.

```cpp
// Rule 4.3 Implementation
int GetPyramidingCount(long magic) {
    int count = 0;
    for(int i = PositionsTotal() - 1; i >= 0; i--) {
        if(PositionSelectByTicket(PositionGetTicket(i))) {
            if(PositionGetInteger(POSITION_MAGIC) == magic && PositionGetString(POSITION_SYMBOL) == _Symbol) count++;
        }
    }
    return count;
}
```

---

## [SILENT_TRAPS_CHECKLIST]

Critical checks to prevent logic corruption.

1. **[TRAP_1] Floating Point Drift:** Normalize all prices to `_Digits`.  
   `double sl_price = NormalizeDouble(Bid - 100 * _Point, _Digits);`

2. **[TRAP_2] Recursive Drift:** Ensure incremental calculation for EMA/RMA.  
   `double currentEMA = (close[i] - prevEMA) * alpha + prevEMA;`

3. **[TRAP_3] Implicit NaN:** Use `MathIsValidNumber()` to mimic Pine's `na` propagation.

4. **[TRAP_4] Array Direction Consistency:** Mixing series and non-series indices leads to signal inversion.  
   `if(!ArrayGetAsSeries(myBuffer)) ArraySetAsSeries(myBuffer, true);`

5. **[TRAP_5] Integer Division:** Pine `5/2 = 2.5`, MQL5 `5/2 = 2`. Use explicit casting `(double)x/y`.  
   `double ratio = (double)current_index / total_count;`

---

## [REFERENCE_DOCUMENTATION]

For detailed implementation patterns and ready-to-use code snippets, refer to:

* [**Snippets Library**](https://github.com/GeoKFX/MQL5_Snippets_and_Skills/blob/main/skills/Pine-Script-to-MQL5-Conversion/references/Pine-to-MQL5_Snippets_library.md)**:** A comprehensive collection of MQL5 code fragments for state persistence, MTF handling, and ECN-compatible trading.
```

