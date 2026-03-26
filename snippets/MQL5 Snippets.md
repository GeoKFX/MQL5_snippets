# MQL5 Snippets (12)

### OnStart
```mql5
int OnStart()
{
   
}
```

---

### OnStart2
```mql5
void OnStart()
{
   
}
```

---

### OnInit
```mql5
int OnInit()
{
   
}
```

---

### OnInit2
```mql5
void OnInit()
{
   
}
```

---

### OnDeinit
```mql5
void OnDeinit(const int reason)
{
   
}
```

---

### OnTick
```mql5
void OnTick()
{
   
}
```

---

### OnCalculate
```mql5
int OnCalculate(const int rates_total, const int prev_calculated, const int begin, const double& price[])
{
   
}
```

---

### OnCalculate2
```mql5
int OnCalculate(const int rates_total, const int prev_calculated, const datetime& time{}, const double& open[], const double& high[], const double& low[], const double& close[], const long& tick_volume[], const long& volume[], const int& spread[])
{
   
}
```

---

### OnTimer
```mql5
void OnTimer()
{
   
}
```

---

### OnTrade
```mql5
void OnTrade()
{
   
}
```

---

### OnTradeTransaction
```mql5
void OnTradeTransaction(const MqlTradeTransaction& trans, const MqlTradeRequest& request, const MqlTradeResult& result)
{
   
}
```

---

### OnBookEvent
```mql5
void OnBookEvent(const string& symbol)
{
   
}
```

---

### OnChartEvent
```mql5
void OnChartEvent(const int id, const long& lparam, const double& dparam, const string& sparam)
{
   
}
```

---

### OnTester
```mql5
double OnTester()
{
   
}
```

---

### OnTesterInit
```mql5
int OnTesterInit()
{
   
}
```

---

### OnTesterInit2
```mql5
void OnTesterInit()
{
   
}
```

---

### OnTesterDeinit
```mql5
void OnTesterDeinit()
{
   
}
```

---

### OnTesterPass
```mql5
void OnTesterPass()
{
   
}
```

---

### OrderCalcMargin
```mql5
OrderCalcMargin(ENUM_ORDER_TYPE action, string symbol, double volume, double price, double& margin)
```

---

### OrderCalcProfit
```mql5
OrderCalcProfit(ENUM_ORDER_TYPE action, string symbol, double volume, double price_open, double price_close, double& profit)
```

---

### OrderCheck
```mql5
OrderCheck(MqlTradeRequest& request, MqlTradeCheckResult& result)
```

---

### OrderSend
```mql5
OrderSend(MqlTradeRequest& request, MqlTradeResult& result)
```

---

### OrderSendAsync
```mql5
OrderSendAsync(MqlTradeRequest& request, MqlTradeResult& result)
```

---

### PositionsTotal
```mql5
PositionsTotal()
```

---

### PositionGetSymbol
```mql5
PositionGetSymbol(int index)
```

---

### PositionSelect
```mql5
PositionSelect(string symbol)
```

---

### PositionSelectByTicket
```mql5
PositionSelectByTicket(ulong ticket)
```

---

### PositionGetDouble
```mql5
PositionGetDouble(ENUM_POSITION_PROPERTY_DOUBLE property_id)
```

---

### PositionGetDouble2
```mql5
PositionGetDouble(ENUM_POSITION_PROPERTY_DOUBLE property_id, double& double_var)
```

---

### PositionGetInteger
```mql5
PositionGetInteger(ENUM_POSITION_PROPERTY_INTEGER property_id)
```

---

### PositionGetInteger2
```mql5
PositionGetInteger(ENUM_POSITION_PROPERTY_INTEGER property_id, long& long_var)
```

---

### PositionGetString
```mql5
PositionGetString(ENUM_POSITION_PROPERTY_STRING property_id)
```

---

### PositionGetString2
```mql5
PositionGetString(ENUM_POSITION_PROPERTY_STRING property_id, string& string_var)
```

---

### PositionGetTicket
```mql5
PositionGetTicket(int index)
```

---

### OrdersTotal
```mql5
OrdersTotal()
```

---

### OrderGetTicket
```mql5
OrderGetTicket(int index)
```

---

### OrderSelect
```mql5
OrderSelect(ulong ticket)
```

---

### OrderSelect2
```mql5
OrderSelect(ulong ticket)
```

---

### OrderGetDouble
```mql5
OrderGetDouble(ENUM_ORDER_PROPERTY_DOUBLE property_id)
```

---

### OrderGetDouble2
```mql5
OrderGetDouble(ENUM_ORDER_PROPERTY_DOUBLE property_id, double& double_var)
```

---

### OrderGetInteger
```mql5
OrderGetInteger(ENUM_ORDER_PROPERTY_INTEGER property_id)
```

---

### OrderGetInteger2
```mql5
OrderGetInteger(ENUM_ORDER_PROPERTY_INTEGER property_id, long& long_var)
```

---

### OrderGetString
```mql5
OrderGetString(ENUM_ORDER_PROPERTY_STRING property_id)
```

---

### OrderGetString2
```mql5
OrderGetString(ENUM_ORDER_PROPERTY_STRING property_id, string& string_var)
```

---

### HistorySelect
```mql5
HistorySelect(datetime from_date, datetime to_date)
```

---

### HistorySelectByPosition
```mql5
HistorySelectByPosition(long position_id)
```

---

### HistoryOrderSelect
```mql5
HistoryOrderSelect(ulong ticket)
```

---

### HistoryOrdersTotal
```mql5
HistoryOrdersTotal()
```

---

### HistoryOrderGetTicket
```mql5
HistoryOrderGetTicket(int index)
```

---

### HistoryOrderGetDouble
```mql5
HistoryOrderGetDouble(ulong ticket_number, ENUM_ORDER_PROPERTY_DOUBLE property_id)
```

---

### HistoryOrderGetDouble2
```mql5
HistoryOrderGetDouble(ulong ticket_number, ENUM_ORDER_PROPERTY_DOUBLE property_id, double& double_var)
```

---

### HistoryOrderGetInteger
```mql5
HistoryOrderGetInteger(ulong ticket_number, ENUM_ORDER_PROPERTY_INTEGER property_id)
```

---

### HistoryOrderGetInteger2
```mql5
HistoryOrderGetInteger(ulong ticket_number, ENUM_ORDER_PROPERTY_INTEGER property_id, long& long_var)
```

---

### HistoryOrderGetString
```mql5
HistoryOrderGetString(ulong ticket_number, ENUM_ORDER_PROPERTY_STRING property_id)
```

---

### HistoryOrderGetString2
```mql5
HistoryOrderGetString(ulong ticket_number, ENUM_ORDER_PROPERTY_STRING property_id, string& string_var)
```

---

### HistoryDealSelect
```mql5
HistoryDealSelect(ulong ticket)
```

---

### HistoryDealsTotal
```mql5
HistoryDealsTotal()
```

---

### HistoryDealGetTicket
```mql5
HistoryDealGetTicket(int index)
```

---

### HistoryDealGetDouble
```mql5
HistoryDealGetDouble(ulong ticket_number, ENUM_DEAL_PROPERTY_DOUBLE property_id)
```

---

### HistoryDealGetDouble2
```mql5
HistoryDealGetDouble(ulong ticket_number, ENUM_DEAL_PROPERTY_DOUBLE property_id, double& double_var)
```

---

### HistoryDealGetInteger
```mql5
HistoryDealGetInteger(ulong ticket_number, ENUM_DEAL_PROPERTY_INTEGER property_id)
```

---

### HistoryDealGetInteger2
```mql5
HistoryDealGetInteger(ulong ticket_number, ENUM_DEAL_PROPERTY_INTEGER property_id, long& long_var)
```

---

### HistoryDealGetString
```mql5
HistoryDealGetString(ulong ticket_number, ENUM_DEAL_PROPERTY_STRING property_id)
```

---

### HistoryDealGetString2
```mql5
HistoryDealGetString(ulong ticket_number, ENUM_DEAL_PROPERTY_STRING property_id, string& string_var)
```

---

### ObjectCreate
```mql5
ObjectCreate(long chart_id, string name, ENUM_OBJECT type, sub_window nwin, datetime time1, double price1, ..., datetime timeN=0, double priceN=0, ..., datetime time30=0, double price30=0)
```

---

### ObjectName
```mql5
ObjectName(long chart_id, int pos, int sub_window=-1, int type=-1)
```

---

### ObjectDelete
```mql5
ObjectDelete(long chart_id, string name)
```

---

### ObjectsDeleteAll
```mql5
ObjectsDeleteAll(long chart_id, int sub_window=-1, int type=-1)
```

---

### ObjectsDeleteAll2
```mql5
ObjectsDeleteAll(long chart_id, const string prefix, int sub_window=-1, int object_type=-1)
```

---

### ObjectFind
```mql5
ObjectFind(long chart_id, string name)
```

---

### ObjectGetTimeByValue
```mql5
ObjectGetTimeByValue(long chart_id, string name, double value, int line_id)
```

---

### ObjectGetValueByTime
```mql5
ObjectGetValueByTime(long chart_id, string name, datetime time, int line_id)
```

---

### ObjectMove
```mql5
ObjectMove(long chart_id, string name, int point_index, datetime time, double price)
```

---

### ObjectsTotal
```mql5
ObjectsTotal(long chart_id, int sub_window=-1, int type=-1)
```

---

### ObjectSetDouble
```mql5
ObjectSetDouble(long chart_id, string name, ENUM_OBJECT_PROPERTY_DOUBLE prop_id, double prop_value)
```

---

### ObjectSetDouble2
```mql5
ObjectSetDouble(long chart_id, string name, ENUM_OBJECT_PROPERTY_DOUBLE prop_id, int prop_modifier, double prop_value)
```

---

### ObjectSetInteger
```mql5
ObjectSetInteger(long chart_id, string name, ENUM_OBJECT_PROPERTY_INTEGER prop_id, long prop_value)
```

---

### ObjectSetInteger2
```mql5
ObjectSetInteger(long chart_id, string name, ENUM_OBJECT_PROPERTY_INTEGER prop_id, int prop_modifier, long prop_value)
```

---

### ObjectSetString
```mql5
ObjectSetString(long chart_id, string name, ENUM_OBJECT_PROPERTY_STRING prop_id, string prop_value)
```

---

### ObjectSetString2
```mql5
ObjectSetString(long chart_id, string name, ENUM_OBJECT_PROPERTY_STRING prop_id, int prop_modifier, string prop_value)
```

---

### ObjectGetDouble
```mql5
ObjectGetDouble(long chart_id, string name, ENUM_OBJECT_PROPERTY_DOUBLE prop_id, int prop_modifier=0)
```

---

### ObjectGetDouble2
```mql5
ObjectGetDouble(long chart_id, string name, ENUM_OBJECT_PROPERTY_DOUBLE prop_id, int prop_modifier, double& double_var)
```

---

### ObjectGetInteger
```mql5
ObjectGetInteger(long chart_id, string name, ENUM_OBJECT_PROPERTY_INTEGER prop_id, int prop_modifier=0)
```

---

### ObjectGetInteger2
```mql5
ObjectGetInteger(long chart_id, string name, ENUM_OBJECT_PROPERTY_INTEGER prop_id, int prop_modifier, long& long_var)
```

---

### ObjectGetString
```mql5
ObjectGetString(long chart_id, string name, ENUM_OBJECT_PROPERTY_STRING prop_id, int prop_modifier=0)
```

---

### ObjectGetString2
```mql5
ObjectGetString(long chart_id, string name, ENUM_OBJECT_PROPERTY_STRING prop_id, int prop_modifier, string& string_var)
```

---

### TextSetFont
```mql5
TextSetFont(const string name, int size, uint flags, int orientation=0)
```

---

### TextOut
```mql5
TextOut(const string text, int x, int y, uint anchor, uint &data[], uint width, uint height, uint color, ENUM_COLOR_FORMAT color_format)
```

---

### TextGetSize
```mql5
TextGetSize(const string text, uint& width, uint& height)
```

---

### iBars
```mql5
iBars(const string symbol, ENUM_TIMEFRAMES timeframe)
```

---

### iBarShift
```mql5
iBarShift(const string symbol, ENUM_TIMEFRAMES timeframe, datetime time, bool exact=false)
```

---

### iClose
```mql5
iClose(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iHigh
```mql5
iHigh(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iHighest
```mql5
iHighest(const string symbol, ENUM_TIMEFRAMES timeframe, ENUM_SERIESMODE type, int count=WHOLE_ARRAY, int start=0)
```

---

### iLow
```mql5
iLow(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iLowest
```mql5
iLowest(const string symbol, ENUM_TIMEFRAMES timeframe, ENUM_SERIESMODE type, int count=WHOLE_ARRAY, int start=0)
```

---

### iOpen
```mql5
iOpen(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iTime
```mql5
iTime(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iTickVolume
```mql5
iTickVolume(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iRealVolume
```mql5
iRealVolume(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iVolume
```mql5
iVolume(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### iSpread
```mql5
iSpread(const string symbol, ENUM_TIMEFRAMES timeframe, int shift)
```

---

### ChartApplyTemplate
```mql5
ChartApplyTemplate(long chart_id, const string filename)
```

---

### ChartSaveTemplate
```mql5
ChartSaveTemplate(long chart_id, const string filename)
```

---

### ChartWindowFind
```mql5
ChartWindowFind(long chart_id, string indicator_shortname)
```

---

### ChartWindowFind2
```mql5
ChartWindowFind()
```

---

### ChartTimePriceToXY
```mql5
ChartTimePriceToXY(long chart_id, int sub_window, datetime time, double price, int& x, int& y)
```

---

### ChartXYToTimePrice
```mql5
ChartXYToTimePrice(long chart_id, int x, int y, int& sub_window, datetime& time, double& price)
```

---

### ChartOpen
```mql5
ChartOpen(string symbol, ENUM_TIMEFRAMES period)
```

---

### ChartFirst
```mql5
ChartFirst()
```

---

### ChartNext
```mql5
ChartNext(long chart_id)
```

---

### ChartClose
```mql5
ChartClose(long chart_id=0)
```

---

### ChartSymbol
```mql5
ChartSymbol(long chart_id=0)
```

---

### ChartPeriod
```mql5
ChartPeriod(long chart_id=0)
```

---

### ChartRedraw
```mql5
ChartRedraw(long chart_id=0)
```

---

### ChartSetDouble
```mql5
ChartSetDouble(long chart_id, int prop_id, double value)
```

---

### ChartSetInteger
```mql5
ChartSetInteger(long chart_id, int prop_id, long value)
```

---

### ChartSetInteger2
```mql5
ChartSetInteger(long chart_id, int prop_id, int sub_window, long value)
```

---

### ChartSetString
```mql5
ChartSetString(long chart_id, int prop_id, string str_value)
```

---

### ChartGetDouble
```mql5
ChartGetDouble(long chart_id, int prop_id, int sub_window=0)
```

---

### ChartGetDouble2
```mql5
ChartGetDouble(long chart_id, int prop_id, int sub_window, double& double_var)
```

---

### ChartGetInteger
```mql5
ChartGetInteger(long chart_id, int prop_id, int sub_window=0)
```

---

### ChartGetInteger2
```mql5
ChartGetInteger(long chart_id, int prop_id, int sub_window, long& long_var)
```

---

### ChartGetString
```mql5
ChartGetString(long chart_id, int prop_id)
```

---

### ChartGetString2
```mql5
ChartGetString(long chart_id, int prop_id, string& string_var)
```

---

### ChartNavigate
```mql5
ChartNavigate(long chart_id, ENUM_CHART_POSITION position, int shift=0)
```

---

### ChartID
```mql5
ChartID()
```

---

### ChartIndicatorAdd
```mql5
ChartIndicatorAdd(long chart_id, int sub_window, int indicator_handle)
```

---

### ChartIndicatorDelete
```mql5
ChartIndicatorDelete(long chart_id, int sub_window, const string indicator_shortname)
```

---

### ChartIndicatorGet
```mql5
ChartIndicatorGet(long chart_id, int sub_window, const string indicator_shortname)
```

---

### ChartIndicatorName
```mql5
ChartIndicatorName(long chart_id, int sub_window, int index)
```

---

### ChartIndicatorsTotal
```mql5
ChartIndicatorsTotal(long chart_id, int sub_window)
```

---

### ChartWindowOnDropped
```mql5
ChartWindowOnDropped()
```

---

### ChartPriceOnDropped
```mql5
ChartPriceOnDropped()
```

---

### ChartTimeOnDropped
```mql5
ChartTimeOnDropped()
```

---

### ChartXOnDropped
```mql5
ChartXOnDropped()
```

---

### ChartYOnDropped
```mql5
ChartYOnDropped()
```

---

### ChartSetSymbolPeriod
```mql5
ChartSetSymbolPeriod(long chart_id, string symbol, ENUM_TIMEFRAMES period)
```

---

### ChartScreenShot
```mql5
ChartScreenShot(long chart_id, string filename, int width, int height, ENUM_ALIGN_MODE align_mode=ALIGN_RIGHT)
```

---

### iAC
```mql5
iAC(string symbol, ENUM_TIMEFRAMES period)
```

---

### iAD
```mql5
iAD(string symbol, ENUM_TIMEFRAMES period, ENUM_APPLIED_VOLUME applied_volume)
```

---

### iADX
```mql5
iADX(string symbol, ENUM_TIMEFRAMES period, int adx_period)
```

---

### iADXWilder
```mql5
iADXWilder(string symbol, ENUM_TIMEFRAMES period, int adx_period)
```

---

### iAlligator
```mql5
iAlligator(string symbol, ENUM_TIMEFRAMES period, int jaw_period, int jaw_shift, int teeth_period, int teeth_shift, int lips_period, int lips_shift, ENUM_MA_METHOD ma_method, ENUM_APPLIED_PRICE applied_price)
```

---

### iAMA
```mql5
iAMA(string symbol, ENUM_TIMEFRAMES period, int ama_period, int fast_ma_period, int slow_ma_period, int ama_shift, ENUM_APPLIED_PRICE applied_price)
```

---

### iAO
```mql5
iAO(string symbol, ENUM_TIMEFRAMES period)
```

---

### iATR
```mql5
iATR(string symbol, ENUM_TIMEFRAMES period, int ma_period)
```

---

### iBearsPower
```mql5
iBearsPower(string symbol, ENUM_TIMEFRAMES period, int ma_period)
```

---

### iBands
```mql5
iBands(string symbol, ENUM_TIMEFRAMES period, int bands_period, int bands_shift, double deviation, ENUM_APPLIED_PRICE applied_price)
```

---

### iBullsPower
```mql5
iBullsPower(string symbol, ENUM_TIMEFRAMES period, int ma_period)
```

---

### iCCI
```mql5
iCCI(string symbol, ENUM_TIMEFRAMES period, int ma_period, ENUM_APPLIED_PRICE applied_price)
```

---

### iChaikin
```mql5
iChaikin(string symbol, ENUM_TIMEFRAMES period, int fast_ma_period, int slow_ma_period, ENUM_MA_METHOD ma_method, ENUM_APPLIED_VOLUME applied_volume)
```

---

### iCustom
```mql5
iCustom(string symbol, ENUM_TIMEFRAMES period, string name, ...)
```

---

### iDEMA
```mql5
iDEMA(string symbol, ENUM_TIMEFRAMES period, int ma_period, int ma_shift, ENUM_APPLIED_PRICE applied_price)
```

---

### iDeMarker
```mql5
iDeMarker(string symbol, ENUM_TIMEFRAMES period, int ma_period)
```

---

### iEnvelopes
```mql5
iEnvelopes(string symbol, ENUM_TIMEFRAMES period, int ma_period, int ma_shift, ENUM_MA_METHOD ma_method, ENUM_APPLIED_PRICE applied_price, double deviation)
```

---

### iForce
```mql5
iForce(string symbol, ENUM_TIMEFRAMES period, int ma_period, ENUM_MA_METHOD ma_method, ENUM_APPLIED_VOLUME applied_volume)
```

---

### iFractals
```mql5
iFractals(string symbol, ENUM_TIMEFRAMES period)
```

---

### iFrAMA
```mql5
iFrAMA(string symbol, ENUM_TIMEFRAMES period, int ma_period, int ma_shift, ENUM_APPLIED_PRICE applied_price)
```

---

### iGator
```mql5
iGator(string symbol, ENUM_TIMEFRAMES period, int jaw_period, int jaw_shift, int teeth_period, int teeth_shift, int lips_period, int lips_shift, ENUM_MA_METHOD ma_method, ENUM_APPLIED_PRICE applied_price)
```

---

### iIchimoku
```mql5
iIchimoku(string symbol, ENUM_TIMEFRAMES period, int tenkan_sen, int kijun_sen, int senkou_span_b)
```

---

### iBWMFI
```mql5
iBWMFI(string symbol, ENUM_TIMEFRAMES period, ENUM_APPLIED_VOLUME applied_volume)
```

---

### iMomentum
```mql5
iMomentum(string symbol, ENUM_TIMEFRAMES period, int mom_period, ENUM_APPLIED_PRICE applied_price)
```

---

### iMFI
```mql5
iMFI(string symbol, ENUM_TIMEFRAMES period, int ma_period, ENUM_APPLIED_VOLUME applied_volume)
```

---

### iMA
```mql5
iMA(string symbol, ENUM_TIMEFRAMES period, int ma_period, int ma_shift, ENUM_MA_METHOD ma_method, ENUM_APPLIED_PRICE applied_price)
```

---

### iOsMA
```mql5
iOsMA(string symbol, ENUM_TIMEFRAMES period, int fast_ema_period, int slow_ema_period, int signal_period, ENUM_APPLIED_PRICE applied_price)
```

---

### iMACD
```mql5
iMACD(string symbol, ENUM_TIMEFRAMES period, int fast_ema_period, int slow_ema_period, int signal_period, ENUM_APPLIED_PRICE applied_price)
```

---

### iOBV
```mql5
iOBV(string symbol, ENUM_TIMEFRAMES period, ENUM_APPLIED_VOLUME applied_volume)
```

---

### iSAR
```mql5
iSAR(string symbol, ENUM_TIMEFRAMES period, double step, double maximum)
```

---

### iRSI
```mql5
iRSI(string symbol, ENUM_TIMEFRAMES period, int ma_period, ENUM_APPLIED_PRICE applied_price)
```

---

### iRVI
```mql5
iRVI(string symbol, ENUM_TIMEFRAMES period, int ma_period)
```

---

### iStdDev
```mql5
iStdDev(string symbol, ENUM_TIMEFRAMES period, int ma_period, int ma_shift, ENUM_MA_METHOD ma_method, ENUM_APPLIED_PRICE applied_price)
```

---

### iStochastic
```mql5
iStochastic(string symbol, ENUM_TIMEFRAMES period, int Kperiod, int Dperiod, int slowing, ENUM_MA_METHOD ma_method, ENUM_STO_PRICE price_field)
```

---

### iTEMA
```mql5
iTEMA(string symbol, ENUM_TIMEFRAMES period, int ma_period, int ma_shift, ENUM_APPLIED_PRICE applied_price)
```

---

### iTriX
```mql5
iTriX(string symbol, ENUM_TIMEFRAMES period, int ma_period, ENUM_APPLIED_PRICE applied_price)
```

---

### iWPR
```mql5
iWPR(string symbol, ENUM_TIMEFRAMES period, int calc_period)
```

---

### iVIDyA
```mql5
iVIDyA(string symbol, ENUM_TIMEFRAMES period, int cmo_period, int ema_period, int ma_shift, ENUM_APPLIED_PRICE applied_price)
```

---

### iVolumes
```mql5
iVolumes(string symbol, ENUM_TIMEFRAMES period, ENUM_APPLIED_VOLUME applied_volume)
```

---

### MathAbs
```mql5
MathAbs(double value)
```

---

### MathArccos
```mql5
MathArccos(double val)
```

---

### MathArcsin
```mql5
MathArcsin(double val)
```

---

### MathArctan
```mql5
MathArctan(double value)
```

---

### MathArctan2
```mql5
MathArctan2(double y, double x)
```

---

### MathClassify
```mql5
MathClassify(double value)
```

---

### MathCeil
```mql5
MathCeil(double val)
```

---

### MathCos
```mql5
MathCos(double value)
```

---

### MathExp
```mql5
MathExp(double value)
```

---

### MathFloor
```mql5
MathFloor(double val)
```

---

### MathLog
```mql5
MathLog(double val)
```

---

### MathLog10
```mql5
MathLog10(double val)
```

---

### MathMax
```mql5
MathMax(double value1, double value2)
```

---

### MathMin
```mql5
MathMin(double value1, double value2)
```

---

### MathMod
```mql5
MathMod(double value, double value2)
```

---

### MathPow
```mql5
MathPow(double base, double exponent)
```

---

### MathRand
```mql5
MathRand()
```

---

### MathRound
```mql5
MathRound(double value)
```

---

### MathSin
```mql5
MathSin(double value)
```

---

### MathSqrt
```mql5
MathSqrt(double value)
```

---

### MathSrand
```mql5
MathSrand(int seed)
```

---

### MathTan
```mql5
MathTan(double rad)
```

---

### MathIsValidNumber
```mql5
MathIsValidNumber(double number)
```

---

### MathExpm1
```mql5
MathExpm1(double value)
```

---

### MathLog1p
```mql5
MathLog1p(double value)
```

---

### MathArccosh
```mql5
MathArccosh(double value)
```

---

### MathArcsinh
```mql5
MathArcsinh(double value)
```

---

### MathArctanh
```mql5
MathArctanh(double value)
```

---

### MathCosh
```mql5
MathCosh(double value)
```

---

### MathSinh
```mql5
MathSinh(double value)
```

---

### MathTanh
```mql5
MathTanh(double value)
```

---

### MathSwap
```mql5
MathSwap(ushort value)
```

---

### MathSwap2
```mql5
MathSwap(uint value)
```

---

### MathSwap3
```mql5
MathSwap(ulong value)
```

---

### GlobalVariableCheck
```mql5
GlobalVariableCheck(string name)
```

---

### GlobalVariableTime
```mql5
GlobalVariableTime(string name)
```

---

### GlobalVariableDel
```mql5
GlobalVariableDel(string name)
```

---

### GlobalVariableGet
```mql5
GlobalVariableGet(string name)
```

---

### GlobalVariableGet2
```mql5
GlobalVariableGet(string name, double& double_var)
```

---

### GlobalVariableName
```mql5
GlobalVariableName(int index)
```

---

### GlobalVariableSet
```mql5
GlobalVariableSet(string name, double value)
```

---

### GlobalVariablesFlush
```mql5
GlobalVariablesFlush()
```

---

### GlobalVariableTemp
```mql5
GlobalVariableTemp(string name)
```

---

### GlobalVariableSetOnCondition
```mql5
GlobalVariableSetOnCondition(string name, double value, double check_value)
```

---

### GlobalVariablesDeleteAll
```mql5
GlobalVariablesDeleteAll(string prefix_name=NULL, datetime limit_data=0)
```

---

### GlobalVariablesTotal
```mql5
GlobalVariablesTotal()
```

---

### FileSelectDialog
```mql5
FileSelectDialog(string caption, string initial_dir, string filter, uint flags, string& filenames[], string default_filename)
```

---

### FileFindFirst
```mql5
FileFindFirst(const string file_filter, string& returned_filename, int common_flag=0)
```

---

### FileFindNext
```mql5
FileFindNext(long search_handle, string& returned_filename)
```

---

### FileFindClose
```mql5
FileFindClose(long search_handle)
```

---

### FileIsExist
```mql5
FileIsExist(const string file_name, int common_flag=0)
```

---

### FileOpen
```mql5
FileOpen(string file_name, int open_flags, short delimiter='	', uint codepage=CP_ACP)
```

---

### FileClose
```mql5
FileClose(int file_handle)
```

---

### FileCopy
```mql5
FileCopy(const string src_file_name, int common_flag, const string dst_file_name, int mode_flags)
```

---

### FileDelete
```mql5
FileDelete(const string file_name, int common_flag=0)
```

---

### FileMove
```mql5
FileMove(const string src_file_name, int common_flag, const string dst_file_name, int mode_flags)
```

---

### FileFlush
```mql5
FileFlush(int file_handle)
```

---

### FileGetInteger
```mql5
FileGetInteger(int file_handle, ENUM_FILE_PROPERTY_INTEGER property_id)
```

---

### FileGetInteger2
```mql5
FileGetInteger(const string file_name, ENUM_FILE_PROPERTY_INTEGER property_id, bool common_folder=false)
```

---

### FileIsEnding
```mql5
FileIsEnding(int file_handle)
```

---

### FileIsLineEnding
```mql5
FileIsLineEnding(int file_handle)
```

---

### FileReadArray
```mql5
FileReadArray(int file_handle, void& array[], int start=0, int count=WHOLE_ARRAY)
```

---

### FileReadBool
```mql5
FileReadBool(int file_handle)
```

---

### FileReadDatetime
```mql5
FileReadDatetime(int file_handle)
```

---

### FileReadDouble
```mql5
FileReadDouble(int file_handle)
```

---

### FileReadFloat
```mql5
FileReadFloat(int file_handle)
```

---

### FileReadInteger
```mql5
FileReadInteger(int file_handle, int size=INT_VALUE)
```

---

### FileReadLong
```mql5
FileReadLong(int file_handle)
```

---

### FileReadNumber
```mql5
FileReadNumber(int file_handle)
```

---

### FileReadString
```mql5
FileReadString(int file_handle, int length=-1)
```

---

### FileReadStruct
```mql5
FileReadStruct(int file_handle, const void& struct_object, int size=-1)
```

---

### FileSeek
```mql5
FileSeek(int file_handle, long offset, ENUM_FILE_POSITION origin)
```

---

### FileSize
```mql5
FileSize(int file_handle)
```

---

### FileTell
```mql5
FileTell(int file_handle)
```

---

### FileWrite
```mql5
FileWrite(int file_handle, ...)
```

---

### FileWriteArray
```mql5
FileWriteArray(int file_handle, const void& array[], int start=0, int count=WHOLE_ARRAY)
```

---

### FileWriteDouble
```mql5
FileWriteDouble(int file_handle, double value)
```

---

### FileWriteFloat
```mql5
FileWriteFloat(int file_handle, float value)
```

---

### FileWriteInteger
```mql5
FileWriteInteger(int file_handle, int value, int size=INT_VALUE)
```

---

### FileWriteLong
```mql5
FileWriteLong(int file_handle, long value)
```

---

### FileWriteString
```mql5
FileWriteString(int file_handle, const string text_string, int length=-1)
```

---

### FileWriteStruct
```mql5
FileWriteStruct(int file_handle, const void& struct_object, int size=-1)
```

---

### FileLoad
```mql5
FileLoad(const string file_name, void& buffer[], int common_flag=0)
```

---

### FileSave
```mql5
FileSave(const string file_name, void& buffer[], int common_flag=0)
```

---

### FolderCreate
```mql5
FolderCreate(string folder_name, int common_flag=0)
```

---

### FolderDelete
```mql5
FolderDelete(string folder_name, int common_flag=0)
```

---

### FolderClean
```mql5
FolderClean(string folder_name, int common_flag=0)
```

---

### DatabaseOpen
```mql5
DatabaseOpen(string filename, uint flags)
```

---

### DatabaseClose
```mql5
DatabaseClose(int database)
```

---

### DatabaseImport
```mql5
DatabaseImport(int database, const string table, const string filename, uint flags, const string separator, ulong skip_rows, const string skip_comments)
```

---

### DatabaseExport
```mql5
DatabaseExport(int database, const string table_or_sql, const string filename, uint flags, const string separator)
```

---

### DatabasePrint
```mql5
DatabasePrint(int database, const string table_or_sql, uint flags)
```

---

### DatabaseTableExists
```mql5
DatabaseTableExists(int database, string table)
```

---

### DatabaseExecute
```mql5
DatabaseExecute(int database, string sql)
```

---

### DatabasePrepare
```mql5
DatabasePrepare(int database, string sql, ...)
```

---

### DatabaseReset
```mql5
DatabaseReset(int request)
```

---

### DatabaseBind
```mql5
DatabaseBind(int request, int index, T value)
```

---

### DatabaseBind2
```mql5
DatabaseBind(int request, int index, T& array[])
```

---

### DatabaseRead
```mql5
DatabaseRead(int request)
```

---

### DatabaseReadBind
```mql5
DatabaseReadBind(int request, void& struct_object)
```

---

### DatabaseFinalize
```mql5
DatabaseFinalize(int request)
```

---

### DatabaseTransactionBegin
```mql5
DatabaseTransactionBegin(int database)
```

---

### DatabaseTransactionCommit
```mql5
DatabaseTransactionCommit(int database)
```

---

### DatabaseTransactionRollback
```mql5
DatabaseTransactionRollback(int database)
```

---

### DatabaseColumnsCount
```mql5
DatabaseColumnsCount(int request)
```

---

### DatabaseColumnName
```mql5
DatabaseColumnName(int request, int column, string& name)
```

---

### DatabaseColumnType
```mql5
DatabaseColumnType(int request, int column)
```

---

### DatabaseColumnSize
```mql5
DatabaseColumnSize(int request, int column)
```

---

### DatabaseColumnText
```mql5
DatabaseColumnText(int request, int column, string& value)
```

---

### DatabaseColumnInteger
```mql5
DatabaseColumnInteger(int request, int column, int& value)
```

---

### DatabaseColumnLong
```mql5
DatabaseColumnLong(int request, int column, long& value)
```

---

### DatabaseColumnDouble
```mql5
DatabaseColumnDouble(int request, int column, double& value)
```

---

### DatabaseColumnBlob
```mql5
DatabaseColumnBlob(int request, int column, void& data[])
```

---

### ENUM_POSITION_PROPERTY_INTEGER
```mql5
ENUM_POSITION_PROPERTY_INTEGER
```

---

### POSITION_TICKET
```mql5
POSITION_TICKET
```

---

### POSITION_TIME
```mql5
POSITION_TIME
```

---

### POSITION_TIME_MSC
```mql5
POSITION_TIME_MSC
```

---

### POSITION_TIME_UPDATE
```mql5
POSITION_TIME_UPDATE
```

---

### POSITION_TIME_UPDATE_MSC
```mql5
POSITION_TIME_UPDATE_MSC
```

---

### POSITION_TYPE
```mql5
POSITION_TYPE
```

---

### POSITION_MAGIC
```mql5
POSITION_MAGIC
```

---

### POSITION_IDENTIFIER
```mql5
POSITION_IDENTIFIER
```

---

### POSITION_REASON
```mql5
POSITION_REASON
```

---

### ENUM_POSITION_PROPERTY_DOUBLE
```mql5
ENUM_POSITION_PROPERTY_DOUBLE
```

---

### POSITION_VOLUME
```mql5
POSITION_VOLUME
```

---

### POSITION_PRICE_OPEN
```mql5
POSITION_PRICE_OPEN
```

---

### POSITION_SL
```mql5
POSITION_SL
```

---

### POSITION_TP
```mql5
POSITION_TP
```

---

### POSITION_PRICE_CURRENT
```mql5
POSITION_PRICE_CURRENT
```

---

### POSITION_SWAP
```mql5
POSITION_SWAP
```

---

### POSITION_PROFIT
```mql5
POSITION_PROFIT
```

---

### ENUM_POSITION_PROPERTY_STRING
```mql5
ENUM_POSITION_PROPERTY_STRING
```

---

### POSITION_SYMBOL
```mql5
POSITION_SYMBOL
```

---

### POSITION_COMMENT
```mql5
POSITION_COMMENT
```

---

### POSITION_EXTERNAL_ID
```mql5
POSITION_EXTERNAL_ID
```

---

### ENUM_POSITION_TYPE
```mql5
ENUM_POSITION_TYPE
```

---

### POSITION_TYPE_BUY
```mql5
POSITION_TYPE_BUY
```

---

### POSITION_TYPE_SELL
```mql5
POSITION_TYPE_SELL
```

---

### ENUM_POSITION_REASON
```mql5
ENUM_POSITION_REASON
```

---

### POSITION_REASON_CLIENT
```mql5
POSITION_REASON_CLIENT
```

---

### POSITION_REASON_MOBILE
```mql5
POSITION_REASON_MOBILE
```

---

### POSITION_REASON_WEB
```mql5
POSITION_REASON_WEB
```

---

### POSITION_REASON_EXPERT
```mql5
POSITION_REASON_EXPERT
```

---

### ENUM_ORDER_PROPERTY_INTEGER
```mql5
ENUM_ORDER_PROPERTY_INTEGER
```

---

### ORDER_TICKET
```mql5
ORDER_TICKET
```

---

### ORDER_TIME_SETUP
```mql5
ORDER_TIME_SETUP
```

---

### ORDER_TYPE
```mql5
ORDER_TYPE
```

---

### ORDER_STATE
```mql5
ORDER_STATE
```

---

### ORDER_TIME_EXPIRATION
```mql5
ORDER_TIME_EXPIRATION
```

---

### ORDER_TIME_DONE
```mql5
ORDER_TIME_DONE
```

---

### ORDER_TIME_SETUP_MSC
```mql5
ORDER_TIME_SETUP_MSC
```

---

### ORDER_TIME_DONE_MSC
```mql5
ORDER_TIME_DONE_MSC
```

---

### ORDER_TYPE_FILLING
```mql5
ORDER_TYPE_FILLING
```

---

### ORDER_TYPE_TIME
```mql5
ORDER_TYPE_TIME
```

---

### ORDER_MAGIC
```mql5
ORDER_MAGIC
```

---

### ORDER_REASON
```mql5
ORDER_REASON
```

---

### ORDER_POSITION_ID
```mql5
ORDER_POSITION_ID
```

---

### ORDER_POSITION_BY_ID
```mql5
ORDER_POSITION_BY_ID
```

---

### ENUM_ORDER_PROPERTY_DOUBLE
```mql5
ENUM_ORDER_PROPERTY_DOUBLE
```

---

### ORDER_VOLUME_INITIAL
```mql5
ORDER_VOLUME_INITIAL
```

---

### ORDER_VOLUME_CURRENT
```mql5
ORDER_VOLUME_CURRENT
```

---

### ORDER_PRICE_OPEN
```mql5
ORDER_PRICE_OPEN
```

---

### ORDER_SL
```mql5
ORDER_SL
```

---

### ORDER_TP
```mql5
ORDER_TP
```

---

### ORDER_PRICE_CURRENT
```mql5
ORDER_PRICE_CURRENT
```

---

### ORDER_PRICE_STOPLIMIT
```mql5
ORDER_PRICE_STOPLIMIT
```

---

### ENUM_ORDER_PROPERTY_STRING
```mql5
ENUM_ORDER_PROPERTY_STRING
```

---

### ORDER_SYMBOL
```mql5
ORDER_SYMBOL
```

---

### ORDER_COMMENT
```mql5
ORDER_COMMENT
```

---

### ORDER_EXTERNAL_ID
```mql5
ORDER_EXTERNAL_ID
```

---

### ENUM_ORDER_TYPE
```mql5
ENUM_ORDER_TYPE
```

---

### ORDER_TYPE_BUY
```mql5
ORDER_TYPE_BUY
```

---

### ORDER_TYPE_SELL
```mql5
ORDER_TYPE_SELL
```

---

### ORDER_TYPE_BUY_LIMIT
```mql5
ORDER_TYPE_BUY_LIMIT
```

---

### ORDER_TYPE_SELL_LIMIT
```mql5
ORDER_TYPE_SELL_LIMIT
```

---

### ORDER_TYPE_BUY_STOP
```mql5
ORDER_TYPE_BUY_STOP
```

---

### ORDER_TYPE_SELL_STOP
```mql5
ORDER_TYPE_SELL_STOP
```

---

### ORDER_TYPE_BUY_STOP_LIMIT
```mql5
ORDER_TYPE_BUY_STOP_LIMIT
```

---

### ORDER_TYPE_SELL_STOP_LIMIT
```mql5
ORDER_TYPE_SELL_STOP_LIMIT
```

---

### ORDER_TYPE_CLOSE_BY
```mql5
ORDER_TYPE_CLOSE_BY
```

---

### ENUM_ORDER_STATE
```mql5
ENUM_ORDER_STATE
```

---

### ORDER_STATE_STARTED
```mql5
ORDER_STATE_STARTED
```

---

### ORDER_STATE_PLACED
```mql5
ORDER_STATE_PLACED
```

---

### ORDER_STATE_CANCELED
```mql5
ORDER_STATE_CANCELED
```

---

### ORDER_STATE_PARTIAL
```mql5
ORDER_STATE_PARTIAL
```

---

### ORDER_STATE_FILLED
```mql5
ORDER_STATE_FILLED
```

---

### ORDER_STATE_REJECTED
```mql5
ORDER_STATE_REJECTED
```

---

### ORDER_STATE_EXPIRED
```mql5
ORDER_STATE_EXPIRED
```

---

### ORDER_STATE_REQUEST_ADD
```mql5
ORDER_STATE_REQUEST_ADD
```

---

### ORDER_STATE_REQUEST_MODIFY
```mql5
ORDER_STATE_REQUEST_MODIFY
```

---

### ORDER_STATE_REQUEST_CANCEL
```mql5
ORDER_STATE_REQUEST_CANCEL
```

---

### ENUM_ORDER_TYPE_FILLING
```mql5
ENUM_ORDER_TYPE_FILLING
```

---

### ORDER_FILLING_FOK
```mql5
ORDER_FILLING_FOK
```

---

### ORDER_FILLING_IOC
```mql5
ORDER_FILLING_IOC
```

---

### ORDER_FILLING_RETURN
```mql5
ORDER_FILLING_RETURN
```

---

### ENUM_ORDER_TYPE_TIME
```mql5
ENUM_ORDER_TYPE_TIME
```

---

### ORDER_TIME_GTC
```mql5
ORDER_TIME_GTC
```

---

### ORDER_TIME_DAY
```mql5
ORDER_TIME_DAY
```

---

### ORDER_TIME_SPECIFIED
```mql5
ORDER_TIME_SPECIFIED
```

---

### ORDER_TIME_SPECIFIED_DAY
```mql5
ORDER_TIME_SPECIFIED_DAY
```

---

### ENUM_ORDER_REASON
```mql5
ENUM_ORDER_REASON
```

---

### ORDER_REASON_CLIENT
```mql5
ORDER_REASON_CLIENT
```

---

### ORDER_REASON_MOBILE
```mql5
ORDER_REASON_MOBILE
```

---

### ORDER_REASON_WEB
```mql5
ORDER_REASON_WEB
```

---

### ORDER_REASON_EXPERT
```mql5
ORDER_REASON_EXPERT
```

---

### ORDER_REASON_SL
```mql5
ORDER_REASON_SL
```

---

### ORDER_REASON_TP
```mql5
ORDER_REASON_TP
```

---

### ORDER_REASON_SO
```mql5
ORDER_REASON_SO
```

---

### ENUM_DEAL_PROPERTY_INTEGER
```mql5
ENUM_DEAL_PROPERTY_INTEGER
```

---

### DEAL_TICKET
```mql5
DEAL_TICKET
```

---

### DEAL_ORDER
```mql5
DEAL_ORDER
```

---

### DEAL_TIME
```mql5
DEAL_TIME
```

---

### DEAL_TIME_MSC
```mql5
DEAL_TIME_MSC
```

---

### DEAL_TYPE
```mql5
DEAL_TYPE
```

---

### DEAL_ENTRY
```mql5
DEAL_ENTRY
```

---

### DEAL_MAGIC
```mql5
DEAL_MAGIC
```

---

### DEAL_REASON
```mql5
DEAL_REASON
```

---

### DEAL_POSITION_ID
```mql5
DEAL_POSITION_ID
```

---

### ENUM_DEAL_PROPERTY_DOUBLE
```mql5
ENUM_DEAL_PROPERTY_DOUBLE
```

---

### DEAL_VOLUME
```mql5
DEAL_VOLUME
```

---

### DEAL_PRICE
```mql5
DEAL_PRICE
```

---

### DEAL_COMMISSION
```mql5
DEAL_COMMISSION
```

---

### DEAL_SWAP
```mql5
DEAL_SWAP
```

---

### DEAL_PROFIT
```mql5
DEAL_PROFIT
```

---

### DEAL_FEE
```mql5
DEAL_FEE
```

---

### DEAL_SL
```mql5
DEAL_SL
```

---

### DEAL_TP
```mql5
DEAL_TP
```

---

### ENUM_DEAL_PROPERTY_STRING
```mql5
ENUM_DEAL_PROPERTY_STRING
```

---

### DEAL_SYMBOL
```mql5
DEAL_SYMBOL
```

---

### DEAL_COMMENT
```mql5
DEAL_COMMENT
```

---

### DEAL_EXTERNAL_ID
```mql5
DEAL_EXTERNAL_ID
```

---

### ENUM_DEAL_TYPE
```mql5
ENUM_DEAL_TYPE
```

---

### DEAL_TYPE_BUY
```mql5
DEAL_TYPE_BUY
```

---

### DEAL_TYPE_SELL
```mql5
DEAL_TYPE_SELL
```

---

### DEAL_TYPE_BALANCE
```mql5
DEAL_TYPE_BALANCE
```

---

### DEAL_TYPE_CREDIT
```mql5
DEAL_TYPE_CREDIT
```

---

### DEAL_TYPE_CHARGE
```mql5
DEAL_TYPE_CHARGE
```

---

### DEAL_TYPE_CORRECTION
```mql5
DEAL_TYPE_CORRECTION
```

---

### DEAL_TYPE_BONUS
```mql5
DEAL_TYPE_BONUS
```

---

### DEAL_TYPE_COMMISSION
```mql5
DEAL_TYPE_COMMISSION
```

---

### DEAL_TYPE_COMMISSION_DAILY
```mql5
DEAL_TYPE_COMMISSION_DAILY
```

---

### DEAL_TYPE_COMMISSION_MONTHLY
```mql5
DEAL_TYPE_COMMISSION_MONTHLY
```

---

### DEAL_TYPE_COMMISSION_AGENT_DAILY
```mql5
DEAL_TYPE_COMMISSION_AGENT_DAILY
```

---

### DEAL_TYPE_COMMISSION_AGENT_MONTHLY
```mql5
DEAL_TYPE_COMMISSION_AGENT_MONTHLY
```

---

### DEAL_TYPE_INTEREST
```mql5
DEAL_TYPE_INTEREST
```

---

### DEAL_TYPE_BUY_CANCELED
```mql5
DEAL_TYPE_BUY_CANCELED
```

---

### DEAL_TYPE_SELL_CANCELED
```mql5
DEAL_TYPE_SELL_CANCELED
```

---

### DEAL_DIVIDEND
```mql5
DEAL_DIVIDEND
```

---

### DEAL_DIVIDEND_FRANKED
```mql5
DEAL_DIVIDEND_FRANKED
```

---

### DEAL_TAX
```mql5
DEAL_TAX
```

---

### ENUM_DEAL_ENTRY
```mql5
ENUM_DEAL_ENTRY
```

---

### DEAL_ENTRY_IN
```mql5
DEAL_ENTRY_IN
```

---

### DEAL_ENTRY_OUT
```mql5
DEAL_ENTRY_OUT
```

---

### DEAL_ENTRY_INOUT
```mql5
DEAL_ENTRY_INOUT
```

---

### DEAL_ENTRY_OUT_BY
```mql5
DEAL_ENTRY_OUT_BY
```

---

### ENUM_DEAL_REASON
```mql5
ENUM_DEAL_REASON
```

---

### DEAL_REASON_CLIENT
```mql5
DEAL_REASON_CLIENT
```

---

### DEAL_REASON_MOBILE
```mql5
DEAL_REASON_MOBILE
```

---

### DEAL_REASON_WEB
```mql5
DEAL_REASON_WEB
```

---

### DEAL_REASON_EXPERT
```mql5
DEAL_REASON_EXPERT
```

---

### DEAL_REASON_SL
```mql5
DEAL_REASON_SL
```

---

### DEAL_REASON_TP
```mql5
DEAL_REASON_TP
```

---

### DEAL_REASON_SO
```mql5
DEAL_REASON_SO
```

---

### DEAL_REASON_ROLLOVER
```mql5
DEAL_REASON_ROLLOVER
```

---

### DEAL_REASON_VMARGIN
```mql5
DEAL_REASON_VMARGIN
```

---

### DEAL_REASON_SPLIT
```mql5
DEAL_REASON_SPLIT
```

---

### ENUM_TRADE_REQUEST_ACTIONS
```mql5
ENUM_TRADE_REQUEST_ACTIONS
```

---

### TRADE_ACTION_DEAL
```mql5
TRADE_ACTION_DEAL
```

---

### TRADE_ACTION_PENDING
```mql5
TRADE_ACTION_PENDING
```

---

### TRADE_ACTION_SLTP
```mql5
TRADE_ACTION_SLTP
```

---

### TRADE_ACTION_MODIFY
```mql5
TRADE_ACTION_MODIFY
```

---

### TRADE_ACTION_REMOVE
```mql5
TRADE_ACTION_REMOVE
```

---

### TRADE_ACTION_CLOSE_BY
```mql5
TRADE_ACTION_CLOSE_BY
```

---

### ENUM_TRADE_TRANSACTION_TYPE
```mql5
ENUM_TRADE_TRANSACTION_TYPE
```

---

### TRADE_TRANSACTION_ORDER_ADD
```mql5
TRADE_TRANSACTION_ORDER_ADD
```

---

### TRADE_TRANSACTION_ORDER_UPDATE
```mql5
TRADE_TRANSACTION_ORDER_UPDATE
```

---

### TRADE_TRANSACTION_ORDER_DELETE
```mql5
TRADE_TRANSACTION_ORDER_DELETE
```

---

### TRADE_TRANSACTION_DEAL_ADD
```mql5
TRADE_TRANSACTION_DEAL_ADD
```

---

### TRADE_TRANSACTION_DEAL_UPDATE
```mql5
TRADE_TRANSACTION_DEAL_UPDATE
```

---

### TRADE_TRANSACTION_DEAL_DELETE
```mql5
TRADE_TRANSACTION_DEAL_DELETE
```

---

### TRADE_TRANSACTION_HISTORY_ADD
```mql5
TRADE_TRANSACTION_HISTORY_ADD
```

---

### TRADE_TRANSACTION_HISTORY_UPDATE
```mql5
TRADE_TRANSACTION_HISTORY_UPDATE
```

---

### TRADE_TRANSACTION_HISTORY_DELETE
```mql5
TRADE_TRANSACTION_HISTORY_DELETE
```

---

### TRADE_TRANSACTION_POSITION
```mql5
TRADE_TRANSACTION_POSITION
```

---

### TRADE_TRANSACTION_REQUEST
```mql5
TRADE_TRANSACTION_REQUEST
```

---

### ENUM_BOOK_TYPE
```mql5
ENUM_BOOK_TYPE
```

---

### BOOK_TYPE_SELL
```mql5
BOOK_TYPE_SELL
```

---

### BOOK_TYPE_BUY
```mql5
BOOK_TYPE_BUY
```

---

### BOOK_TYPE_SELL_MARKET
```mql5
BOOK_TYPE_SELL_MARKET
```

---

### BOOK_TYPE_BUY_MARKET
```mql5
BOOK_TYPE_BUY_MARKET
```

---

### ENUM_SIGNAL_BASE_DOUBLE
```mql5
ENUM_SIGNAL_BASE_DOUBLE
```

---

### SIGNAL_BASE_BALANCE
```mql5
SIGNAL_BASE_BALANCE
```

---

### SIGNAL_BASE_EQUITY
```mql5
SIGNAL_BASE_EQUITY
```

---

### SIGNAL_BASE_GAIN
```mql5
SIGNAL_BASE_GAIN
```

---

### SIGNAL_BASE_MAX_DRAWDOWN
```mql5
SIGNAL_BASE_MAX_DRAWDOWN
```

---

### SIGNAL_BASE_PRICE
```mql5
SIGNAL_BASE_PRICE
```

---

### SIGNAL_BASE_ROI
```mql5
SIGNAL_BASE_ROI
```

---

### ENUM_SIGNAL_BASE_INTEGER
```mql5
ENUM_SIGNAL_BASE_INTEGER
```

---

### SIGNAL_BASE_DATE_PUBLISHED
```mql5
SIGNAL_BASE_DATE_PUBLISHED
```

---

### SIGNAL_BASE_DATE_STARTED
```mql5
SIGNAL_BASE_DATE_STARTED
```

---

### SIGNAL_BASE_DATE_UPDATED
```mql5
SIGNAL_BASE_DATE_UPDATED
```

---

### SIGNAL_BASE_ID
```mql5
SIGNAL_BASE_ID
```

---

### SIGNAL_BASE_LEVERAGE
```mql5
SIGNAL_BASE_LEVERAGE
```

---

### SIGNAL_BASE_PIPS
```mql5
SIGNAL_BASE_PIPS
```

---

### SIGNAL_BASE_RATING
```mql5
SIGNAL_BASE_RATING
```

---

### SIGNAL_BASE_SUBSCRIBERS
```mql5
SIGNAL_BASE_SUBSCRIBERS
```

---

### SIGNAL_BASE_TRADES
```mql5
SIGNAL_BASE_TRADES
```

---

### SIGNAL_BASE_TRADE_MODE
```mql5
SIGNAL_BASE_TRADE_MODE
```

---

### ENUM_SIGNAL_BASE_STRING
```mql5
ENUM_SIGNAL_BASE_STRING
```

---

### SIGNAL_BASE_AUTHOR_LOGIN
```mql5
SIGNAL_BASE_AUTHOR_LOGIN
```

---

### SIGNAL_BASE_BROKER
```mql5
SIGNAL_BASE_BROKER
```

---

### SIGNAL_BASE_BROKER_SERVER
```mql5
SIGNAL_BASE_BROKER_SERVER
```

---

### SIGNAL_BASE_NAME
```mql5
SIGNAL_BASE_NAME
```

---

### SIGNAL_BASE_CURRENCY
```mql5
SIGNAL_BASE_CURRENCY
```

---

### ENUM_SIGNAL_INFO_DOUBLE
```mql5
ENUM_SIGNAL_INFO_DOUBLE
```

---

### SIGNAL_INFO_EQUITY_LIMIT
```mql5
SIGNAL_INFO_EQUITY_LIMIT
```

---

### SIGNAL_INFO_SLIPPAGE
```mql5
SIGNAL_INFO_SLIPPAGE
```

---

### SIGNAL_INFO_VOLUME_PERCENT
```mql5
SIGNAL_INFO_VOLUME_PERCENT
```

---

### ENUM_SIGNAL_INFO_INTEGER
```mql5
ENUM_SIGNAL_INFO_INTEGER
```

---

### SIGNAL_INFO_CONFIRMATIONS_DISABLED
```mql5
SIGNAL_INFO_CONFIRMATIONS_DISABLED
```

---

### SIGNAL_INFO_COPY_SLTP
```mql5
SIGNAL_INFO_COPY_SLTP
```

---

### SIGNAL_INFO_DEPOSIT_PERCENT
```mql5
SIGNAL_INFO_DEPOSIT_PERCENT
```

---

### SIGNAL_INFO_ID
```mql5
SIGNAL_INFO_ID
```

---

### SIGNAL_INFO_SUBSCRIPTION_ENABLED
```mql5
SIGNAL_INFO_SUBSCRIPTION_ENABLED
```

---

### SIGNAL_INFO_TERMS_AGREE
```mql5
SIGNAL_INFO_TERMS_AGREE
```

---

### ENUM_SIGNAL_INFO_STRING
```mql5
ENUM_SIGNAL_INFO_STRING
```

---

### SIGNAL_INFO_NAME
```mql5
SIGNAL_INFO_NAME
```

---

### ENUM_SERIES_INFO_INTEGER
```mql5
ENUM_SERIES_INFO_INTEGER
```

---

### SERIES_BARS_COUNT
```mql5
SERIES_BARS_COUNT
```

---

### SERIES_FIRSTDATE
```mql5
SERIES_FIRSTDATE
```

---

### SERIES_LASTBAR_DATE
```mql5
SERIES_LASTBAR_DATE
```

---

### SERIES_SERVER_FIRSTDATE
```mql5
SERIES_SERVER_FIRSTDATE
```

---

### SERIES_TERMINAL_FIRSTDATE
```mql5
SERIES_TERMINAL_FIRSTDATE
```

---

### SERIES_SYNCHRONIZED
```mql5
SERIES_SYNCHRONIZED
```

---

### ENUM_CHART_EVENT
```mql5
ENUM_CHART_EVENT
```

---

### CHARTEVENT_KEYDOWN
```mql5
CHARTEVENT_KEYDOWN
```

---

### CHARTEVENT_MOUSE_MOVE
```mql5
CHARTEVENT_MOUSE_MOVE
```

---

### CHARTEVENT_MOUSE_WHEEL
```mql5
CHARTEVENT_MOUSE_WHEEL
```

---

### CHARTEVENT_OBJECT_CREATE
```mql5
CHARTEVENT_OBJECT_CREATE
```

---

### CHARTEVENT_OBJECT_CHANGE
```mql5
CHARTEVENT_OBJECT_CHANGE
```

---

### CHARTEVENT_OBJECT_DELETE
```mql5
CHARTEVENT_OBJECT_DELETE
```

---

### CHARTEVENT_CLICK
```mql5
CHARTEVENT_CLICK
```

---

### CHARTEVENT_OBJECT_CLICK
```mql5
CHARTEVENT_OBJECT_CLICK
```

---

### CHARTEVENT_OBJECT_DRAG
```mql5
CHARTEVENT_OBJECT_DRAG
```

---

### CHARTEVENT_OBJECT_ENDEDIT
```mql5
CHARTEVENT_OBJECT_ENDEDIT
```

---

### CHARTEVENT_CHART_CHANGE
```mql5
CHARTEVENT_CHART_CHANGE
```

---

### CHARTEVENT_CUSTOM
```mql5
CHARTEVENT_CUSTOM
```

---

### CHARTEVENT_CUSTOM_LAST
```mql5
CHARTEVENT_CUSTOM_LAST
```

---

### ENUM_TIMEFRAMES
```mql5
ENUM_TIMEFRAMES
```

---

### PERIOD_CURRENT
```mql5
PERIOD_CURRENT
```

---

### PERIOD_M1
```mql5
PERIOD_M1
```

---

### PERIOD_M2
```mql5
PERIOD_M2
```

---

### PERIOD_M3
```mql5
PERIOD_M3
```

---

### PERIOD_M4
```mql5
PERIOD_M4
```

---

### PERIOD_M5
```mql5
PERIOD_M5
```

---

### PERIOD_M6
```mql5
PERIOD_M6
```

---

### PERIOD_M10
```mql5
PERIOD_M10
```

---

### PERIOD_M12
```mql5
PERIOD_M12
```

---

### PERIOD_M15
```mql5
PERIOD_M15
```

---

### PERIOD_M20
```mql5
PERIOD_M20
```

---

### PERIOD_M30
```mql5
PERIOD_M30
```

---

### PERIOD_H1
```mql5
PERIOD_H1
```

---

### PERIOD_H2
```mql5
PERIOD_H2
```

---

### PERIOD_H3
```mql5
PERIOD_H3
```

---

### PERIOD_H4
```mql5
PERIOD_H4
```

---

### PERIOD_H6
```mql5
PERIOD_H6
```

---

### PERIOD_H8
```mql5
PERIOD_H8
```

---

### PERIOD_H12
```mql5
PERIOD_H12
```

---

### PERIOD_D1
```mql5
PERIOD_D1
```

---

### PERIOD_W1
```mql5
PERIOD_W1
```

---

### PERIOD_MN1
```mql5
PERIOD_MN1
```

---

### ENUM_SERIESMODE
```mql5
ENUM_SERIESMODE
```

---

### MODE_OPEN
```mql5
MODE_OPEN
```

---

### MODE_LOW
```mql5
MODE_LOW
```

---

### MODE_HIGH
```mql5
MODE_HIGH
```

---

### MODE_CLOSE
```mql5
MODE_CLOSE
```

---

### MODE_VOLUME
```mql5
MODE_VOLUME
```

---

### MODE_REAL_VOLUME
```mql5
MODE_REAL_VOLUME
```

---

### MODE_SPREAD
```mql5
MODE_SPREAD
```

---

### ENUM_CHART_PROPERTY_INTEGER
```mql5
ENUM_CHART_PROPERTY_INTEGER
```

---

### CHART_SHOW
```mql5
CHART_SHOW
```

---

### CHART_IS_OBJECT
```mql5
CHART_IS_OBJECT
```

---

### CHART_BRING_TO_TOP
```mql5
CHART_BRING_TO_TOP
```

---

### CHART_CONTEXT_MENU
```mql5
CHART_CONTEXT_MENU
```

---

### CHART_CROSSHAIR_TOOL
```mql5
CHART_CROSSHAIR_TOOL
```

---

### CHART_MOUSE_SCROLL
```mql5
CHART_MOUSE_SCROLL
```

---

### CHART_EVENT_MOUSE_WHEEL
```mql5
CHART_EVENT_MOUSE_WHEEL
```

---

### CHART_EVENT_MOUSE_MOVE
```mql5
CHART_EVENT_MOUSE_MOVE
```

---

### CHART_EVENT_OBJECT_CREATE
```mql5
CHART_EVENT_OBJECT_CREATE
```

---

### CHART_EVENT_OBJECT_DELETE
```mql5
CHART_EVENT_OBJECT_DELETE
```

---

### CHART_MODE
```mql5
CHART_MODE
```

---

### CHART_FOREGROUND
```mql5
CHART_FOREGROUND
```

---

### CHART_SHIFT
```mql5
CHART_SHIFT
```

---

### CHART_AUTOSCROLL
```mql5
CHART_AUTOSCROLL
```

---

### CHART_KEYBOARD_CONTROL
```mql5
CHART_KEYBOARD_CONTROL
```

---

### CHART_QUICK_NAVIGATION
```mql5
CHART_QUICK_NAVIGATION
```

---

### CHART_SCALE
```mql5
CHART_SCALE
```

---

### CHART_SCALEFIX
```mql5
CHART_SCALEFIX
```

---

### CHART_SCALEFIX_11
```mql5
CHART_SCALEFIX_11
```

---

### CHART_SCALE_PT_PER_BAR
```mql5
CHART_SCALE_PT_PER_BAR
```

---

### CHART_SHOW_TICKER
```mql5
CHART_SHOW_TICKER
```

---

### CHART_SHOW_OHLC
```mql5
CHART_SHOW_OHLC
```

---

### CHART_SHOW_BID_LINE
```mql5
CHART_SHOW_BID_LINE
```

---

### CHART_SHOW_ASK_LINE
```mql5
CHART_SHOW_ASK_LINE
```

---

### CHART_SHOW_LAST_LINE
```mql5
CHART_SHOW_LAST_LINE
```

---

### CHART_SHOW_PERIOD_SEP
```mql5
CHART_SHOW_PERIOD_SEP
```

---

### CHART_SHOW_GRID
```mql5
CHART_SHOW_GRID
```

---

### CHART_SHOW_VOLUMES
```mql5
CHART_SHOW_VOLUMES
```

---

### CHART_SHOW_OBJECT_DESCR
```mql5
CHART_SHOW_OBJECT_DESCR
```

---

### CHART_VISIBLE_BARS
```mql5
CHART_VISIBLE_BARS
```

---

### CHART_WINDOWS_TOTAL
```mql5
CHART_WINDOWS_TOTAL
```

---

### CHART_WINDOW_IS_VISIBLE
```mql5
CHART_WINDOW_IS_VISIBLE
```

---

### CHART_WINDOW_HANDLE
```mql5
CHART_WINDOW_HANDLE
```

---

### CHART_WINDOW_YDISTANCE
```mql5
CHART_WINDOW_YDISTANCE
```

---

### CHART_FIRST_VISIBLE_BAR
```mql5
CHART_FIRST_VISIBLE_BAR
```

---

### CHART_WIDTH_IN_BARS
```mql5
CHART_WIDTH_IN_BARS
```

---

### CHART_WIDTH_IN_PIXELS
```mql5
CHART_WIDTH_IN_PIXELS
```

---

### CHART_HEIGHT_IN_PIXELS
```mql5
CHART_HEIGHT_IN_PIXELS
```

---

### CHART_COLOR_BACKGROUND
```mql5
CHART_COLOR_BACKGROUND
```

---

### CHART_COLOR_FOREGROUND
```mql5
CHART_COLOR_FOREGROUND
```

---

### CHART_COLOR_GRID
```mql5
CHART_COLOR_GRID
```

---

### CHART_COLOR_VOLUME
```mql5
CHART_COLOR_VOLUME
```

---

### CHART_COLOR_CHART_UP
```mql5
CHART_COLOR_CHART_UP
```

---

### CHART_COLOR_CHART_DOWN
```mql5
CHART_COLOR_CHART_DOWN
```

---

### CHART_COLOR_CHART_LINE
```mql5
CHART_COLOR_CHART_LINE
```

---

### CHART_COLOR_CANDLE_BULL
```mql5
CHART_COLOR_CANDLE_BULL
```

---

### CHART_COLOR_CANDLE_BEAR
```mql5
CHART_COLOR_CANDLE_BEAR
```

---

### CHART_COLOR_BID
```mql5
CHART_COLOR_BID
```

---

### CHART_COLOR_ASK
```mql5
CHART_COLOR_ASK
```

---

### CHART_COLOR_LAST
```mql5
CHART_COLOR_LAST
```

---

### CHART_COLOR_STOP_LEVEL
```mql5
CHART_COLOR_STOP_LEVEL
```

---

### CHART_SHOW_TRADE_LEVELS
```mql5
CHART_SHOW_TRADE_LEVELS
```

---

### CHART_DRAG_TRADE_LEVELS
```mql5
CHART_DRAG_TRADE_LEVELS
```

---

### CHART_SHOW_DATE_SCALE
```mql5
CHART_SHOW_DATE_SCALE
```

---

### CHART_SHOW_PRICE_SCALE
```mql5
CHART_SHOW_PRICE_SCALE
```

---

### CHART_SHOW_ONE_CLICK
```mql5
CHART_SHOW_ONE_CLICK
```

---

### CHART_IS_MAXIMIZED
```mql5
CHART_IS_MAXIMIZED
```

---

### CHART_IS_MINIMIZED
```mql5
CHART_IS_MINIMIZED
```

---

### CHART_IS_DOCKED
```mql5
CHART_IS_DOCKED
```

---

### CHART_FLOAT_LEFT
```mql5
CHART_FLOAT_LEFT
```

---

### CHART_FLOAT_TOP
```mql5
CHART_FLOAT_TOP
```

---

### CHART_FLOAT_RIGHT
```mql5
CHART_FLOAT_RIGHT
```

---

### CHART_FLOAT_BOTTOM
```mql5
CHART_FLOAT_BOTTOM
```

---

### ENUM_CHART_PROPERTY_DOUBLE
```mql5
ENUM_CHART_PROPERTY_DOUBLE
```

---

### CHART_SHIFT_SIZE
```mql5
CHART_SHIFT_SIZE
```

---

### CHART_FIXED_POSITION
```mql5
CHART_FIXED_POSITION
```

---

### CHART_FIXED_MAX
```mql5
CHART_FIXED_MAX
```

---

### CHART_FIXED_MIN
```mql5
CHART_FIXED_MIN
```

---

### CHART_POINTS_PER_BAR
```mql5
CHART_POINTS_PER_BAR
```

---

### CHART_PRICE_MIN
```mql5
CHART_PRICE_MIN
```

---

### CHART_PRICE_MAX
```mql5
CHART_PRICE_MAX
```

---

### ENUM_CHART_PROPERTY_STRING
```mql5
ENUM_CHART_PROPERTY_STRING
```

---

### CHART_COMMENT
```mql5
CHART_COMMENT
```

---

### CHART_EXPERT_NAME
```mql5
CHART_EXPERT_NAME
```

---

### CHART_SCRIPT_NAME
```mql5
CHART_SCRIPT_NAME
```

---

### ENUM_CHART_POSITION
```mql5
ENUM_CHART_POSITION
```

---

### CHART_BEGIN
```mql5
CHART_BEGIN
```

---

### CHART_CURRENT_POS
```mql5
CHART_CURRENT_POS
```

---

### CHART_END
```mql5
CHART_END
```

---

### ENUM_CHART_MODE
```mql5
ENUM_CHART_MODE
```

---

### CHART_BARS
```mql5
CHART_BARS
```

---

### CHART_CANDLES
```mql5
CHART_CANDLES
```

---

### CHART_LINE
```mql5
CHART_LINE
```

---

### ENUM_CHART_VOLUME_MODE
```mql5
ENUM_CHART_VOLUME_MODE
```

---

### CHART_VOLUME_HIDE
```mql5
CHART_VOLUME_HIDE
```

---

### CHART_VOLUME_TICK
```mql5
CHART_VOLUME_TICK
```

---

### CHART_VOLUME_REAL
```mql5
CHART_VOLUME_REAL
```

---

### ENUM_OBJECT
```mql5
ENUM_OBJECT
```

---

### OBJ_VLINE
```mql5
OBJ_VLINE
```

---

### OBJ_HLINEl Line
```mql5
OBJ_HLINEl Line
```

---

### OBJ_TREND
```mql5
OBJ_TREND
```

---

### OBJ_TRENDBYANGLE
```mql5
OBJ_TRENDBYANGLE
```

---

### OBJ_CYCLES
```mql5
OBJ_CYCLES
```

---

### OBJ_ARROWED_LINE
```mql5
OBJ_ARROWED_LINE
```

---

### OBJ_CHANNEL
```mql5
OBJ_CHANNEL
```

---

### OBJ_STDDEVCHANNEL
```mql5
OBJ_STDDEVCHANNEL
```

---

### OBJ_REGRESSION
```mql5
OBJ_REGRESSION
```

---

### OBJ_PITCHFORK
```mql5
OBJ_PITCHFORK
```

---

### OBJ_GANNLINE
```mql5
OBJ_GANNLINE
```

---

### OBJ_GANNFAN
```mql5
OBJ_GANNFAN
```

---

### OBJ_GANNGRID
```mql5
OBJ_GANNGRID
```

---

### OBJ_FIBO
```mql5
OBJ_FIBO
```

---

### OBJ_FIBOTIMES
```mql5
OBJ_FIBOTIMES
```

---

### OBJ_FIBOFAN
```mql5
OBJ_FIBOFAN
```

---

### OBJ_FIBOARC
```mql5
OBJ_FIBOARC
```

---

### OBJ_FIBOCHANNEL
```mql5
OBJ_FIBOCHANNEL
```

---

### OBJ_EXPANSION
```mql5
OBJ_EXPANSION
```

---

### OBJ_ELLIOTWAVE5
```mql5
OBJ_ELLIOTWAVE5
```

---

### OBJ_ELLIOTWAVE3
```mql5
OBJ_ELLIOTWAVE3
```

---

### OBJ_RECTANGLE
```mql5
OBJ_RECTANGLE
```

---

### OBJ_TRIANGLE
```mql5
OBJ_TRIANGLE
```

---

### OBJ_ELLIPSE
```mql5
OBJ_ELLIPSE
```

---

### OBJ_ARROW_THUMB_UP
```mql5
OBJ_ARROW_THUMB_UP
```

---

### OBJ_ARROW_THUMB_DOWN
```mql5
OBJ_ARROW_THUMB_DOWN
```

---

### OBJ_ARROW_UP
```mql5
OBJ_ARROW_UP
```

---

### OBJ_ARROW_DOWN
```mql5
OBJ_ARROW_DOWN
```

---

### OBJ_ARROW_STOP
```mql5
OBJ_ARROW_STOP
```

---

### OBJ_ARROW_CHECK
```mql5
OBJ_ARROW_CHECK
```

---

### OBJ_ARROW_LEFT_PRICE
```mql5
OBJ_ARROW_LEFT_PRICE
```

---

### OBJ_ARROW_RIGHT_PRICE
```mql5
OBJ_ARROW_RIGHT_PRICE
```

---

### OBJ_ARROW_BUY
```mql5
OBJ_ARROW_BUY
```

---

### OBJ_ARROW_SELL
```mql5
OBJ_ARROW_SELL
```

---

### OBJ_ARROW
```mql5
OBJ_ARROW
```

---

### OBJ_TEXT
```mql5
OBJ_TEXT
```

---

### OBJ_LABEL
```mql5
OBJ_LABEL
```

---

### OBJ_BUTTON
```mql5
OBJ_BUTTON
```

---

### OBJ_CHART
```mql5
OBJ_CHART
```

---

### OBJ_BITMAP
```mql5
OBJ_BITMAP
```

---

### OBJ_BITMAP_LABEL
```mql5
OBJ_BITMAP_LABEL
```

---

### OBJ_EDIT
```mql5
OBJ_EDIT
```

---

### OBJ_EVENT
```mql5
OBJ_EVENT
```

---

### OBJ_RECTANGLE_LABEL
```mql5
OBJ_RECTANGLE_LABEL
```

---

### ENUM_OBJECT_PROPERTY_INTEGER
```mql5
ENUM_OBJECT_PROPERTY_INTEGER
```

---

### OBJPROP_COLOR
```mql5
OBJPROP_COLOR
```

---

### OBJPROP_STYLE
```mql5
OBJPROP_STYLE
```

---

### OBJPROP_WIDTH
```mql5
OBJPROP_WIDTH
```

---

### OBJPROP_BACK
```mql5
OBJPROP_BACK
```

---

### OBJPROP_ZORDER
```mql5
OBJPROP_ZORDER
```

---

### OBJPROP_FILL
```mql5
OBJPROP_FILL
```

---

### OBJPROP_HIDDEN
```mql5
OBJPROP_HIDDEN
```

---

### OBJPROP_SELECTED
```mql5
OBJPROP_SELECTED
```

---

### OBJPROP_READONLY
```mql5
OBJPROP_READONLY
```

---

### OBJPROP_TYPE
```mql5
OBJPROP_TYPE
```

---

### OBJPROP_TIME
```mql5
OBJPROP_TIME
```

---

### OBJPROP_SELECTABLE
```mql5
OBJPROP_SELECTABLE
```

---

### OBJPROP_CREATETIME
```mql5
OBJPROP_CREATETIME
```

---

### OBJPROP_LEVELS
```mql5
OBJPROP_LEVELS
```

---

### OBJPROP_LEVELCOLOR
```mql5
OBJPROP_LEVELCOLOR
```

---

### OBJPROP_LEVELSTYLE
```mql5
OBJPROP_LEVELSTYLE
```

---

### OBJPROP_LEVELWIDTH
```mql5
OBJPROP_LEVELWIDTH
```

---

### OBJPROP_ALIGN
```mql5
OBJPROP_ALIGN
```

---

### OBJPROP_FONTSIZE
```mql5
OBJPROP_FONTSIZE
```

---

### OBJPROP_RAY_LEFT
```mql5
OBJPROP_RAY_LEFT
```

---

### OBJPROP_RAY_RIGHT
```mql5
OBJPROP_RAY_RIGHT
```

---

### OBJPROP_RAY
```mql5
OBJPROP_RAY
```

---

### OBJPROP_ELLIPSE
```mql5
OBJPROP_ELLIPSE
```

---

### OBJPROP_ARROWCODE
```mql5
OBJPROP_ARROWCODE
```

---

### OBJPROP_TIMEFRAMES
```mql5
OBJPROP_TIMEFRAMES
```

---

### OBJPROP_ANCHOR
```mql5
OBJPROP_ANCHOR
```

---

### OBJPROP_XDISTANCE
```mql5
OBJPROP_XDISTANCE
```

---

### OBJPROP_YDISTANCE
```mql5
OBJPROP_YDISTANCE
```

---

### OBJPROP_DIRECTION
```mql5
OBJPROP_DIRECTION
```

---

### OBJPROP_DEGREE
```mql5
OBJPROP_DEGREE
```

---

### OBJPROP_DRAWLINES
```mql5
OBJPROP_DRAWLINES
```

---

### OBJPROP_STATE
```mql5
OBJPROP_STATE
```

---

### OBJPROP_CHART_ID
```mql5
OBJPROP_CHART_ID
```

---

### OBJPROP_XSIZE
```mql5
OBJPROP_XSIZE
```

---

### OBJPROP_YSIZE
```mql5
OBJPROP_YSIZE
```

---

### OBJPROP_XOFFSET
```mql5
OBJPROP_XOFFSET
```

---

### OBJPROP_YOFFSET
```mql5
OBJPROP_YOFFSET
```

---

### OBJPROP_PERIOD
```mql5
OBJPROP_PERIOD
```

---

### OBJPROP_DATE_SCALE
```mql5
OBJPROP_DATE_SCALE
```

---

### OBJPROP_PRICE_SCALE
```mql5
OBJPROP_PRICE_SCALE
```

---

### OBJPROP_CHART_SCALE
```mql5
OBJPROP_CHART_SCALE
```

---

### OBJPROP_BGCOLOR
```mql5
OBJPROP_BGCOLOR
```

---

### OBJPROP_CORNER
```mql5
OBJPROP_CORNER
```

---

### OBJPROP_BORDER_TYPE
```mql5
OBJPROP_BORDER_TYPE
```

---

### OBJPROP_BORDER_COLOR
```mql5
OBJPROP_BORDER_COLOR
```

---

### ENUM_OBJECT_PROPERTY_DOUBLE
```mql5
ENUM_OBJECT_PROPERTY_DOUBLE
```

---

### OBJPROP_PRICE
```mql5
OBJPROP_PRICE
```

---

### OBJPROP_LEVELVALUE
```mql5
OBJPROP_LEVELVALUE
```

---

### OBJPROP_SCALE
```mql5
OBJPROP_SCALE
```

---

### OBJPROP_ANGLE
```mql5
OBJPROP_ANGLE
```

---

### OBJPROP_DEVIATION
```mql5
OBJPROP_DEVIATION
```

---

### ENUM_OBJECT_PROPERTY_STRING
```mql5
ENUM_OBJECT_PROPERTY_STRING
```

---

### OBJPROP_NAME
```mql5
OBJPROP_NAME
```

---

### OBJPROP_TEXT
```mql5
OBJPROP_TEXT
```

---

### OBJPROP_TOOLTIP
```mql5
OBJPROP_TOOLTIP
```

---

### OBJPROP_LEVELTEXT
```mql5
OBJPROP_LEVELTEXT
```

---

### OBJPROP_FONT
```mql5
OBJPROP_FONT
```

---

### OBJPROP_BMPFILE
```mql5
OBJPROP_BMPFILE
```

---

### OBJPROP_SYMBOL
```mql5
OBJPROP_SYMBOL
```

---

### ENUM_BORDER_TYPE
```mql5
ENUM_BORDER_TYPE
```

---

### BORDER_FLAT
```mql5
BORDER_FLAT
```

---

### BORDER_RAISED
```mql5
BORDER_RAISED
```

---

### BORDER_SUNKEN
```mql5
BORDER_SUNKEN
```

---

### ENUM_ALIGN_MODE
```mql5
ENUM_ALIGN_MODE
```

---

### ALIGN_LEFT
```mql5
ALIGN_LEFT
```

---

### ALIGN_CENTER
```mql5
ALIGN_CENTER
```

---

### ALIGN_RIGHT
```mql5
ALIGN_RIGHT
```

---

### ENUM_ANCHOR_POINT
```mql5
ENUM_ANCHOR_POINT
```

---

### ANCHOR_LEFT_UPPER
```mql5
ANCHOR_LEFT_UPPER
```

---

### ANCHOR_LEFT
```mql5
ANCHOR_LEFT
```

---

### ANCHOR_LEFT_LOWER
```mql5
ANCHOR_LEFT_LOWER
```

---

### ANCHOR_LOWER
```mql5
ANCHOR_LOWER
```

---

### ANCHOR_RIGHT_LOWER
```mql5
ANCHOR_RIGHT_LOWER
```

---

### ANCHOR_RIGHT
```mql5
ANCHOR_RIGHT
```

---

### ANCHOR_RIGHT_UPPER
```mql5
ANCHOR_RIGHT_UPPER
```

---

### ANCHOR_UPPER
```mql5
ANCHOR_UPPER
```

---

### ANCHOR_CENTER
```mql5
ANCHOR_CENTER
```

---

### ENUM_ARROW_ANCHOR
```mql5
ENUM_ARROW_ANCHOR
```

---

### ANCHOR_TOP
```mql5
ANCHOR_TOP
```

---

### ANCHOR_BOTTOM
```mql5
ANCHOR_BOTTOM
```

---

### ENUM_BASE_CORNER
```mql5
ENUM_BASE_CORNER
```

---

### CORNER_LEFT_UPPER
```mql5
CORNER_LEFT_UPPER
```

---

### CORNER_LEFT_LOWER
```mql5
CORNER_LEFT_LOWER
```

---

### CORNER_RIGHT_LOWER
```mql5
CORNER_RIGHT_LOWER
```

---

### CORNER_RIGHT_UPPER
```mql5
CORNER_RIGHT_UPPER
```

---

### OBJ_NO_PERIODS
```mql5
OBJ_NO_PERIODS
```

---

### OBJ_PERIOD_M1
```mql5
OBJ_PERIOD_M1
```

---

### OBJ_PERIOD_M2
```mql5
OBJ_PERIOD_M2
```

---

### OBJ_PERIOD_M3
```mql5
OBJ_PERIOD_M3
```

---

### OBJ_PERIOD_M4
```mql5
OBJ_PERIOD_M4
```

---

### OBJ_PERIOD_M5
```mql5
OBJ_PERIOD_M5
```

---

### OBJ_PERIOD_M6
```mql5
OBJ_PERIOD_M6
```

---

### OBJ_PERIOD_M10
```mql5
OBJ_PERIOD_M10
```

---

### OBJ_PERIOD_M12
```mql5
OBJ_PERIOD_M12
```

---

### OBJ_PERIOD_M15
```mql5
OBJ_PERIOD_M15
```

---

### OBJ_PERIOD_M20
```mql5
OBJ_PERIOD_M20
```

---

### OBJ_PERIOD_M30
```mql5
OBJ_PERIOD_M30
```

---

### OBJ_PERIOD_H1
```mql5
OBJ_PERIOD_H1
```

---

### OBJ_PERIOD_H2
```mql5
OBJ_PERIOD_H2
```

---

### OBJ_PERIOD_H3
```mql5
OBJ_PERIOD_H3
```

---

### OBJ_PERIOD_H4
```mql5
OBJ_PERIOD_H4
```

---

### OBJ_PERIOD_H6
```mql5
OBJ_PERIOD_H6
```

---

### OBJ_PERIOD_H8
```mql5
OBJ_PERIOD_H8
```

---

### OBJ_PERIOD_H12
```mql5
OBJ_PERIOD_H12
```

---

### OBJ_PERIOD_D1
```mql5
OBJ_PERIOD_D1
```

---

### OBJ_PERIOD_W1
```mql5
OBJ_PERIOD_W1
```

---

### OBJ_PERIOD_MN1
```mql5
OBJ_PERIOD_MN1
```

---

### OBJ_ALL_PERIODS
```mql5
OBJ_ALL_PERIODS
```

---

### ENUM_ELLIOT_WAVE_DEGREE
```mql5
ENUM_ELLIOT_WAVE_DEGREE
```

---

### ELLIOTT_GRAND_SUPERCYCLE
```mql5
ELLIOTT_GRAND_SUPERCYCLE
```

---

### ELLIOTT_SUPERCYCLE
```mql5
ELLIOTT_SUPERCYCLE
```

---

### ELLIOTT_CYCLE
```mql5
ELLIOTT_CYCLE
```

---

### ELLIOTT_PRIMARY
```mql5
ELLIOTT_PRIMARY
```

---

### ELLIOTT_INTERMEDIATE
```mql5
ELLIOTT_INTERMEDIATE
```

---

### ELLIOTT_MINOR
```mql5
ELLIOTT_MINOR
```

---

### ELLIOTT_MINUTE
```mql5
ELLIOTT_MINUTE
```

---

### ELLIOTT_MINUETTE
```mql5
ELLIOTT_MINUETTE
```

---

### ELLIOTT_SUBMINUETTE
```mql5
ELLIOTT_SUBMINUETTE
```

---

### ENUM_GANN_DIRECTION
```mql5
ENUM_GANN_DIRECTION
```

---

### GANN_UP_TREND
```mql5
GANN_UP_TREND
```

---

### GANN_DOWN_TREND
```mql5
GANN_DOWN_TREND
```

---

### clrBlack
```mql5
clrBlack
```

---

### clrDarkGreen
```mql5
clrDarkGreen
```

---

### clrDarkSlateGray
```mql5
clrDarkSlateGray
```

---

### clrOlive
```mql5
clrOlive
```

---

### clrGreen
```mql5
clrGreen
```

---

### clrTeal
```mql5
clrTeal
```

---

### clrNavy
```mql5
clrNavy
```

---

### clrPurple
```mql5
clrPurple
```

---

### clrMaroon
```mql5
clrMaroon
```

---

### clrIndigo
```mql5
clrIndigo
```

---

### clrMidnightBlue
```mql5
clrMidnightBlue
```

---

### clrDarkBlue
```mql5
clrDarkBlue
```

---

### clrDarkOliveGreen
```mql5
clrDarkOliveGreen
```

---

### clrSaddleBrown
```mql5
clrSaddleBrown
```

---

### clrForestGreen
```mql5
clrForestGreen
```

---

### clrOliveDrab
```mql5
clrOliveDrab
```

---

### clrSeaGreen
```mql5
clrSeaGreen
```

---

### clrDarkGoldenrod
```mql5
clrDarkGoldenrod
```

---

### clrDarkSlateBlue
```mql5
clrDarkSlateBlue
```

---

### clrSienna
```mql5
clrSienna
```

---

### clrMediumBlue
```mql5
clrMediumBlue
```

---

### clrBrown
```mql5
clrBrown
```

---

### clrDarkTurquoise
```mql5
clrDarkTurquoise
```

---

### clrDimGray
```mql5
clrDimGray
```

---

### clrLightSeaGreen
```mql5
clrLightSeaGreen
```

---

### clrDarkViolet
```mql5
clrDarkViolet
```

---

### clrFireBrick
```mql5
clrFireBrick
```

---

### clrMediumVioletRed
```mql5
clrMediumVioletRed
```

---

### clrMediumSeaGreen
```mql5
clrMediumSeaGreen
```

---

### clrChocolate
```mql5
clrChocolate
```

---

### clrCrimson
```mql5
clrCrimson
```

---

### clrSteelBlue
```mql5
clrSteelBlue
```

---

### clrGoldenrod
```mql5
clrGoldenrod
```

---

### clrMediumSpringGreen
```mql5
clrMediumSpringGreen
```

---

### clrLawnGreen
```mql5
clrLawnGreen
```

---

### clrCadetBlue
```mql5
clrCadetBlue
```

---

### clrDarkOrchid
```mql5
clrDarkOrchid
```

---

### clrYellowGreen
```mql5
clrYellowGreen
```

---

### clrLimeGreen
```mql5
clrLimeGreen
```

---

### clrOrangeRed
```mql5
clrOrangeRed
```

---

### clrDarkOrange
```mql5
clrDarkOrange
```

---

### clrOrange
```mql5
clrOrange
```

---

### clrGold
```mql5
clrGold
```

---

### clrYellow
```mql5
clrYellow
```

---

### clrChartreuse
```mql5
clrChartreuse
```

---

### clrLime
```mql5
clrLime
```

---

### clrSpringGreen
```mql5
clrSpringGreen
```

---

### clrAqua
```mql5
clrAqua
```

---

### clrDeepSkyBlue
```mql5
clrDeepSkyBlue
```

---

### clrBlue
```mql5
clrBlue
```

---

### clrMagenta
```mql5
clrMagenta
```

---

### clrRed
```mql5
clrRed
```

---

### clrGray
```mql5
clrGray
```

---

### clrSlateGray
```mql5
clrSlateGray
```

---

### clrPeru
```mql5
clrPeru
```

---

### clrBlueViolet
```mql5
clrBlueViolet
```

---

### clrLightSlateGray
```mql5
clrLightSlateGray
```

---

### clrDeepPink
```mql5
clrDeepPink
```

---

### clrMediumTurquoise
```mql5
clrMediumTurquoise
```

---

### clrDodgerBlue
```mql5
clrDodgerBlue
```

---

### clrTurquoise
```mql5
clrTurquoise
```

---

### clrRoyalBlue
```mql5
clrRoyalBlue
```

---

### clrSlateBlue
```mql5
clrSlateBlue
```

---

### clrDarkKhaki
```mql5
clrDarkKhaki
```

---

### clrIndianRed
```mql5
clrIndianRed
```

---

### clrMediumOrchid
```mql5
clrMediumOrchid
```

---

### clrGreenYellow
```mql5
clrGreenYellow
```

---

### clrMediumAquamarine
```mql5
clrMediumAquamarine
```

---

### clrDarkSeaGreen
```mql5
clrDarkSeaGreen
```

---

### clrTomato
```mql5
clrTomato
```

---

### clrRosyBrown
```mql5
clrRosyBrown
```

---

### clrOrchid
```mql5
clrOrchid
```

---

### clrMediumurple
```mql5
clrMediumurple
```

---

### clrPaleVioletRed
```mql5
clrPaleVioletRed
```

---

### clrCoral
```mql5
clrCoral
```

---

### clrCornflowerBlue
```mql5
clrCornflowerBlue
```

---

### clrDarkGray
```mql5
clrDarkGray
```

---

### clrSandyBrown
```mql5
clrSandyBrown
```

---

### clrMediumSlateBlue
```mql5
clrMediumSlateBlue
```

---

### clrTan
```mql5
clrTan
```

---

### clrDarkSalmon
```mql5
clrDarkSalmon
```

---

### clrBurlyWood
```mql5
clrBurlyWood
```

---

### clrHotPink
```mql5
clrHotPink
```

---

### clrSalmon
```mql5
clrSalmon
```

---

### clrViolet
```mql5
clrViolet
```

---

### clrLightCoral
```mql5
clrLightCoral
```

---

### clrSkyBlue
```mql5
clrSkyBlue
```

---

### clrLightSalmon
```mql5
clrLightSalmon
```

---

### clrPlum
```mql5
clrPlum
```

---

### clrKhaki
```mql5
clrKhaki
```

---

### clrLightGreen
```mql5
clrLightGreen
```

---

### clrAquamarine
```mql5
clrAquamarine
```

---

### clrSilver
```mql5
clrSilver
```

---

### clrLightSkyBlue
```mql5
clrLightSkyBlue
```

---

### clrLightSteelBlue
```mql5
clrLightSteelBlue
```

---

### clrLightBlue
```mql5
clrLightBlue
```

---

### clrPaleGreen
```mql5
clrPaleGreen
```

---

### clrThistle
```mql5
clrThistle
```

---

### clrPowderBlue
```mql5
clrPowderBlue
```

---

### clrPaleGoldenrod
```mql5
clrPaleGoldenrod
```

---

### clrPaleTurquoise
```mql5
clrPaleTurquoise
```

---

### clrLightGray
```mql5
clrLightGray
```

---

### clrWheat
```mql5
clrWheat
```

---

### clrNavajoWhite
```mql5
clrNavajoWhite
```

---

### clrMoccasin
```mql5
clrMoccasin
```

---

### clrLightPink
```mql5
clrLightPink
```

---

### clrGainsboro
```mql5
clrGainsboro
```

---

### clrPeachPuff
```mql5
clrPeachPuff
```

---

### clrPink
```mql5
clrPink
```

---

### clrBisque
```mql5
clrBisque
```

---

### clrLightGoldenrod
```mql5
clrLightGoldenrod
```

---

### clrBlanchedAlmond
```mql5
clrBlanchedAlmond
```

---

### clrLemonChiffon
```mql5
clrLemonChiffon
```

---

### clrBeige
```mql5
clrBeige
```

---

### clrAntiqueWhite
```mql5
clrAntiqueWhite
```

---

### clrPapayaWhip
```mql5
clrPapayaWhip
```

---

### clrCornsilk
```mql5
clrCornsilk
```

---

### clrLightYellow
```mql5
clrLightYellow
```

---

### clrLightCyan
```mql5
clrLightCyan
```

---

### clrLinen
```mql5
clrLinen
```

---

### clrLavender
```mql5
clrLavender
```

---

### clrMistyRose
```mql5
clrMistyRose
```

---

### clrOldLace
```mql5
clrOldLace
```

---

### clrWhiteSmoke
```mql5
clrWhiteSmoke
```

---

### clrSeashell
```mql5
clrSeashell
```

---

### clrIvory
```mql5
clrIvory
```

---

### clrHoneydew
```mql5
clrHoneydew
```

---

### clrAliceBlue
```mql5
clrAliceBlue
```

---

### clrLavenderBlush
```mql5
clrLavenderBlush
```

---

### clrMintCream
```mql5
clrMintCream
```

---

### clrSnow
```mql5
clrSnow
```

---

### clrWhite
```mql5
clrWhite
```

---

### ENUM_APPLIED_PRICE
```mql5
ENUM_APPLIED_PRICE
```

---

### PRICE_CLOSE
```mql5
PRICE_CLOSE
```

---

### PRICE_OPEN
```mql5
PRICE_OPEN
```

---

### PRICE_HIGH
```mql5
PRICE_HIGH
```

---

### PRICE_LOW
```mql5
PRICE_LOW
```

---

### PRICE_MEDIAN
```mql5
PRICE_MEDIAN
```

---

### PRICE_TYPICAL
```mql5
PRICE_TYPICAL
```

---

### PRICE_WEIGHTED
```mql5
PRICE_WEIGHTED
```

---

### ENUM_APPLIED_VOLUME
```mql5
ENUM_APPLIED_VOLUME
```

---

### VOLUME_TICK
```mql5
VOLUME_TICK
```

---

### VOLUME_REAL
```mql5
VOLUME_REAL
```

---

### ENUM_STO_PRICE
```mql5
ENUM_STO_PRICE
```

---

### STO_LOWHIGH
```mql5
STO_LOWHIGH
```

---

### STO_CLOSECLOSE
```mql5
STO_CLOSECLOSE
```

---

### ENUM_MA_METHOD
```mql5
ENUM_MA_METHOD
```

---

### MODE_SMA
```mql5
MODE_SMA
```

---

### MODE_EMA
```mql5
MODE_EMA
```

---

### MODE_SMMA
```mql5
MODE_SMMA
```

---

### MODE_LWMA
```mql5
MODE_LWMA
```

---

### ENUM_DRAW_TYPE
```mql5
ENUM_DRAW_TYPE
```

---

### DRAW_NONE
```mql5
DRAW_NONE
```

---

### DRAW_LINE
```mql5
DRAW_LINE
```

---

### DRAW_SECTION
```mql5
DRAW_SECTION
```

---

### DRAW_HISTOGRAM
```mql5
DRAW_HISTOGRAM
```

---

### DRAW_HISTOGRAM2
```mql5
DRAW_HISTOGRAM2
```

---

### DRAW_ARROW
```mql5
DRAW_ARROW
```

---

### DRAW_ZIGZAG
```mql5
DRAW_ZIGZAG
```

---

### DRAW_FILLING
```mql5
DRAW_FILLING
```

---

### DRAW_BARS
```mql5
DRAW_BARS
```

---

### DRAW_CANDLES
```mql5
DRAW_CANDLES
```

---

### DRAW_COLOR_LINE
```mql5
DRAW_COLOR_LINE
```

---

### DRAW_COLOR_SECTION
```mql5
DRAW_COLOR_SECTION
```

---

### DRAW_COLOR_HISTOGRAM
```mql5
DRAW_COLOR_HISTOGRAM
```

---

### DRAW_COLOR_HISTOGRAM2
```mql5
DRAW_COLOR_HISTOGRAM2
```

---

### DRAW_COLOR_ARROW
```mql5
DRAW_COLOR_ARROW
```

---

### DRAW_COLOR_ZIGZAG
```mql5
DRAW_COLOR_ZIGZAG
```

---

### DRAW_COLOR_BARS
```mql5
DRAW_COLOR_BARS
```

---

### DRAW_COLOR_CANDLES
```mql5
DRAW_COLOR_CANDLES
```

---

### ENUM_PLOT_PROPERTY_INTEGER
```mql5
ENUM_PLOT_PROPERTY_INTEGER
```

---

### PLOT_ARROW
```mql5
PLOT_ARROW
```

---

### PLOT_ARROW_SHIFT
```mql5
PLOT_ARROW_SHIFT
```

---

### PLOT_DRAW_BEGIN
```mql5
PLOT_DRAW_BEGIN
```

---

### PLOT_DRAW_TYPE
```mql5
PLOT_DRAW_TYPE
```

---

### PLOT_SHOW_DATA
```mql5
PLOT_SHOW_DATA
```

---

### PLOT_SHIFT
```mql5
PLOT_SHIFT
```

---

### PLOT_LINE_STYLE
```mql5
PLOT_LINE_STYLE
```

---

### PLOT_LINE_WIDTH
```mql5
PLOT_LINE_WIDTH
```

---

### PLOT_COLOR_INDEXES
```mql5
PLOT_COLOR_INDEXES
```

---

### PLOT_LINE_COLOR
```mql5
PLOT_LINE_COLOR
```

---

### ENUM_PLOT_PROPERTY_DOUBLE
```mql5
ENUM_PLOT_PROPERTY_DOUBLE
```

---

### PLOT_EMPTY_VALUE
```mql5
PLOT_EMPTY_VALUE
```

---

### ENUM_PLOT_PROPERTY_STRING
```mql5
ENUM_PLOT_PROPERTY_STRING
```

---

### PLOT_LABEL
```mql5
PLOT_LABEL
```

---

### ENUM_LINE_STYLE
```mql5
ENUM_LINE_STYLE
```

---

### STYLE_SOLID
```mql5
STYLE_SOLID
```

---

### STYLE_DASH
```mql5
STYLE_DASH
```

---

### STYLE_DOT
```mql5
STYLE_DOT
```

---

### STYLE_DASHDOT
```mql5
STYLE_DASHDOT
```

---

### STYLE_DASHDOTDOT
```mql5
STYLE_DASHDOTDOT
```

---

### ENUM_INDEXBUFFER_TYPE
```mql5
ENUM_INDEXBUFFER_TYPE
```

---

### INDICATOR_DATA
```mql5
INDICATOR_DATA
```

---

### INDICATOR_COLOR_INDEX
```mql5
INDICATOR_COLOR_INDEX
```

---

### INDICATOR_CALCULATIONS
```mql5
INDICATOR_CALCULATIONS
```

---

### ENUM_CUSTOMIND_PROPERTY_INTEGER
```mql5
ENUM_CUSTOMIND_PROPERTY_INTEGER
```

---

### INDICATOR_DIGITS
```mql5
INDICATOR_DIGITS
```

---

### INDICATOR_HEIGHT
```mql5
INDICATOR_HEIGHT
```

---

### INDICATOR_LEVELS
```mql5
INDICATOR_LEVELS
```

---

### INDICATOR_LEVELCOLOR
```mql5
INDICATOR_LEVELCOLOR
```

---

### INDICATOR_LEVELSTYLE
```mql5
INDICATOR_LEVELSTYLE
```

---

### INDICATOR_LEVELWIDTH
```mql5
INDICATOR_LEVELWIDTH
```

---

### ENUM_CUSTOMIND_PROPERTY_DOUBLE
```mql5
ENUM_CUSTOMIND_PROPERTY_DOUBLE
```

---

### INDICATOR_MINIMUM
```mql5
INDICATOR_MINIMUM
```

---

### INDICATOR_MAXIMUM
```mql5
INDICATOR_MAXIMUM
```

---

### INDICATOR_LEVELVALUE
```mql5
INDICATOR_LEVELVALUE
```

---

### ENUM_CUSTOMIND_PROPERTY_STRING
```mql5
ENUM_CUSTOMIND_PROPERTY_STRING
```

---

### INDICATOR_SHORTNAME
```mql5
INDICATOR_SHORTNAME
```

---

### INDICATOR_LEVELTEXT
```mql5
INDICATOR_LEVELTEXT
```

---

### ENUM_INDICATOR
```mql5
ENUM_INDICATOR
```

---

### IND_AC
```mql5
IND_AC
```

---

### IND_AD
```mql5
IND_AD
```

---

### IND_ADX
```mql5
IND_ADX
```

---

### IND_ADXW
```mql5
IND_ADXW
```

---

### IND_ALLIGATOR
```mql5
IND_ALLIGATOR
```

---

### IND_AMA
```mql5
IND_AMA
```

---

### IND_AO
```mql5
IND_AO
```

---

### IND_ATR
```mql5
IND_ATR
```

---

### IND_BANDS
```mql5
IND_BANDS
```

---

### IND_BEARS
```mql5
IND_BEARS
```

---

### IND_BULLS
```mql5
IND_BULLS
```

---

### IND_BWMFI
```mql5
IND_BWMFI
```

---

### IND_CCI
```mql5
IND_CCI
```

---

### IND_CHAIKIN
```mql5
IND_CHAIKIN
```

---

### IND_CUSTOM
```mql5
IND_CUSTOM
```

---

### IND_DEMA
```mql5
IND_DEMA
```

---

### IND_DEMARKER
```mql5
IND_DEMARKER
```

---

### IND_ENVELOPES
```mql5
IND_ENVELOPES
```

---

### IND_FORCE
```mql5
IND_FORCE
```

---

### IND_FRACTALS
```mql5
IND_FRACTALS
```

---

### IND_FRAMA
```mql5
IND_FRAMA
```

---

### IND_GATOR
```mql5
IND_GATOR
```

---

### IND_ICHIMOKU
```mql5
IND_ICHIMOKU
```

---

### IND_MA
```mql5
IND_MA
```

---

### IND_MACD
```mql5
IND_MACD
```

---

### IND_MFI
```mql5
IND_MFI
```

---

### IND_MOMENTUM
```mql5
IND_MOMENTUM
```

---

### IND_OBV
```mql5
IND_OBV
```

---

### IND_OSMA
```mql5
IND_OSMA
```

---

### IND_RSI
```mql5
IND_RSI
```

---

### IND_RVI
```mql5
IND_RVI
```

---

### IND_SAR
```mql5
IND_SAR
```

---

### IND_STDDEV
```mql5
IND_STDDEV
```

---

### IND_STOCHASTIC
```mql5
IND_STOCHASTIC
```

---

### IND_TEMA
```mql5
IND_TEMA
```

---

### IND_TRIX
```mql5
IND_TRIX
```

---

### IND_VIDYA
```mql5
IND_VIDYA
```

---

### IND_VOLUMES
```mql5
IND_VOLUMES
```

---

### IND_WPR
```mql5
IND_WPR
```

---

### ENUM_DATATYPE
```mql5
ENUM_DATATYPE
```

---

### TYPE_BOOL
```mql5
TYPE_BOOL
```

---

### TYPE_CHAR
```mql5
TYPE_CHAR
```

---

### TYPE_UCHAR
```mql5
TYPE_UCHAR
```

---

### TYPE_SHORT
```mql5
TYPE_SHORT
```

---

### TYPE_USHORT
```mql5
TYPE_USHORT
```

---

### TYPE_COLOR
```mql5
TYPE_COLOR
```

---

### TYPE_INT
```mql5
TYPE_INT
```

---

### TYPE_UINT
```mql5
TYPE_UINT
```

---

### TYPE_DATETIME
```mql5
TYPE_DATETIME
```

---

### TYPE_LONG
```mql5
TYPE_LONG
```

---

### TYPE_ULONG
```mql5
TYPE_ULONG
```

---

### TYPE_FLOAT
```mql5
TYPE_FLOAT
```

---

### TYPE_DOUBLE
```mql5
TYPE_DOUBLE
```

---

### TYPE_STRING
```mql5
TYPE_STRING
```

---

### ENUM_TERMINAL_INFO_INTEGER
```mql5
ENUM_TERMINAL_INFO_INTEGER
```

---

### TERMINAL_BUILD
```mql5
TERMINAL_BUILD
```

---

### TERMINAL_COMMUNITY_ACCOUNT
```mql5
TERMINAL_COMMUNITY_ACCOUNT
```

---

### TERMINAL_COMMUNITY_CONNECTION
```mql5
TERMINAL_COMMUNITY_CONNECTION
```

---

### TERMINAL_CONNECTED
```mql5
TERMINAL_CONNECTED
```

---

### TERMINAL_DLLS_ALLOWED
```mql5
TERMINAL_DLLS_ALLOWED
```

---

### TERMINAL_TRADE_ALLOWED
```mql5
TERMINAL_TRADE_ALLOWED
```

---

### TERMINAL_EMAIL_ENABLED
```mql5
TERMINAL_EMAIL_ENABLED
```

---

### TERMINAL_FTP_ENABLED
```mql5
TERMINAL_FTP_ENABLED
```

---

### TERMINAL_NOTIFICATIONS_ENABLED
```mql5
TERMINAL_NOTIFICATIONS_ENABLED
```

---

### TERMINAL_MAXBARS
```mql5
TERMINAL_MAXBARS
```

---

### TERMINAL_MQID
```mql5
TERMINAL_MQID
```

---

### TERMINAL_CODEPAGE
```mql5
TERMINAL_CODEPAGE
```

---

### TERMINAL_CPU_CORES
```mql5
TERMINAL_CPU_CORES
```

---

### TERMINAL_DISK_SPACE
```mql5
TERMINAL_DISK_SPACE
```

---

### TERMINAL_MEMORY_PHYSICAL
```mql5
TERMINAL_MEMORY_PHYSICAL
```

---

### TERMINAL_MEMORY_TOTAL
```mql5
TERMINAL_MEMORY_TOTAL
```

---

### TERMINAL_MEMORY_AVAILABLE
```mql5
TERMINAL_MEMORY_AVAILABLE
```

---

### TERMINAL_MEMORY_USED
```mql5
TERMINAL_MEMORY_USED
```

---

### TERMINAL_X64
```mql5
TERMINAL_X64
```

---

### TERMINAL_OPENCL_SUPPORT
```mql5
TERMINAL_OPENCL_SUPPORT
```

---

### TERMINAL_SCREEN_DPI
```mql5
TERMINAL_SCREEN_DPI
```

---

### TERMINAL_SCREEN_LEFT
```mql5
TERMINAL_SCREEN_LEFT
```

---

### TERMINAL_SCREEN_TOP
```mql5
TERMINAL_SCREEN_TOP
```

---

### TERMINAL_SCREEN_WIDTH
```mql5
TERMINAL_SCREEN_WIDTH
```

---

### TERMINAL_SCREEN_HEIGHT
```mql5
TERMINAL_SCREEN_HEIGHT
```

---

### TERMINAL_LEFT
```mql5
TERMINAL_LEFT
```

---

### TERMINAL_TOP
```mql5
TERMINAL_TOP
```

---

### TERMINAL_RIGHT
```mql5
TERMINAL_RIGHT
```

---

### TERMINAL_BOTTOM
```mql5
TERMINAL_BOTTOM
```

---

### TERMINAL_PING_LAST
```mql5
TERMINAL_PING_LAST
```

---

### TERMINAL_VPS
```mql5
TERMINAL_VPS
```

---

### TERMINAL_KEYSTATE_LEFT
```mql5
TERMINAL_KEYSTATE_LEFT
```

---

### TERMINAL_KEYSTATE_UP
```mql5
TERMINAL_KEYSTATE_UP
```

---

### TERMINAL_KEYSTATE_RIGHT
```mql5
TERMINAL_KEYSTATE_RIGHT
```

---

### TERMINAL_KEYSTATE_DOWN
```mql5
TERMINAL_KEYSTATE_DOWN
```

---

### TERMINAL_KEYSTATE_SHIFT
```mql5
TERMINAL_KEYSTATE_SHIFT
```

---

### TERMINAL_KEYSTATE_CONTROL
```mql5
TERMINAL_KEYSTATE_CONTROL
```

---

### TERMINAL_KEYSTATE_MENU
```mql5
TERMINAL_KEYSTATE_MENU
```

---

### TERMINAL_KEYSTATE_CAPSLOCK
```mql5
TERMINAL_KEYSTATE_CAPSLOCK
```

---

### TERMINAL_KEYSTATE_NUMLOCK
```mql5
TERMINAL_KEYSTATE_NUMLOCK
```

---

### TERMINAL_KEYSTATE_SCRLOCK
```mql5
TERMINAL_KEYSTATE_SCRLOCK
```

---

### TERMINAL_KEYSTATE_ENTER
```mql5
TERMINAL_KEYSTATE_ENTER
```

---

### TERMINAL_KEYSTATE_INSERT
```mql5
TERMINAL_KEYSTATE_INSERT
```

---

### TERMINAL_KEYSTATE_DELETE
```mql5
TERMINAL_KEYSTATE_DELETE
```

---

### TERMINAL_KEYSTATE_HOME
```mql5
TERMINAL_KEYSTATE_HOME
```

---

### TERMINAL_KEYSTATE_END
```mql5
TERMINAL_KEYSTATE_END
```

---

### TERMINAL_KEYSTATE_TAB
```mql5
TERMINAL_KEYSTATE_TAB
```

---

### TERMINAL_KEYSTATE_PAGEUP
```mql5
TERMINAL_KEYSTATE_PAGEUP
```

---

### TERMINAL_KEYSTATE_PAGEDOWN
```mql5
TERMINAL_KEYSTATE_PAGEDOWN
```

---

### TERMINAL_KEYSTATE_ESCAPE
```mql5
TERMINAL_KEYSTATE_ESCAPE
```

---

### ENUM_TERMINAL_INFO_DOUBLE
```mql5
ENUM_TERMINAL_INFO_DOUBLE
```

---

### TERMINAL_COMMUNITY_BALANCE
```mql5
TERMINAL_COMMUNITY_BALANCE
```

---

### TERMINAL_RETRANSMISSION
```mql5
TERMINAL_RETRANSMISSION
```

---

### ENUM_TERMINAL_INFO_STRING
```mql5
ENUM_TERMINAL_INFO_STRING
```

---

### TERMINAL_LANGUAGE
```mql5
TERMINAL_LANGUAGE
```

---

### TERMINAL_COMPANY
```mql5
TERMINAL_COMPANY
```

---

### TERMINAL_NAME
```mql5
TERMINAL_NAME
```

---

### TERMINAL_PATH
```mql5
TERMINAL_PATH
```

---

### TERMINAL_DATA_PATH
```mql5
TERMINAL_DATA_PATH
```

---

### TERMINAL_COMMONDATA_PATH
```mql5
TERMINAL_COMMONDATA_PATH
```

---

### ENUM_MQL_INFO_INTEGER
```mql5
ENUM_MQL_INFO_INTEGER
```

---

### MQL_HANDLES_USED
```mql5
MQL_HANDLES_USED
```

---

### MQL_MEMORY_LIMIT
```mql5
MQL_MEMORY_LIMIT
```

---

### MQL_MEMORY_USED
```mql5
MQL_MEMORY_USED
```

---

### MQL_PROGRAM_TYPE
```mql5
MQL_PROGRAM_TYPE
```

---

### MQL_DLLS_ALLOWED
```mql5
MQL_DLLS_ALLOWED
```

---

### MQL_TRADE_ALLOWED
```mql5
MQL_TRADE_ALLOWED
```

---

### MQL_SIGNALS_ALLOWED
```mql5
MQL_SIGNALS_ALLOWED
```

---

### MQL_DEBUG
```mql5
MQL_DEBUG
```

---

### MQL_PROFILER
```mql5
MQL_PROFILER
```

---

### MQL_TESTER
```mql5
MQL_TESTER
```

---

### MQL_FORWARD
```mql5
MQL_FORWARD
```

---

### MQL_OPTIMIZATION
```mql5
MQL_OPTIMIZATION
```

---

### MQL_VISUAL_MODE
```mql5
MQL_VISUAL_MODE
```

---

### MQL_FRAME_MODE
```mql5
MQL_FRAME_MODE
```

---

### MQL_LICENSE_TYPE
```mql5
MQL_LICENSE_TYPE
```

---

### ENUM_MQL_INFO_STRING
```mql5
ENUM_MQL_INFO_STRING
```

---

### MQL_PROGRAM_NAME
```mql5
MQL_PROGRAM_NAME
```

---

### MQL5_PROGRAM_PATH
```mql5
MQL5_PROGRAM_PATH
```

---

### ENUM_PROGRAM_TYPE
```mql5
ENUM_PROGRAM_TYPE
```

---

### PROGRAM_SCRIPT
```mql5
PROGRAM_SCRIPT
```

---

### PROGRAM_EXPERT
```mql5
PROGRAM_EXPERT
```

---

### PROGRAM_INDICATOR
```mql5
PROGRAM_INDICATOR
```

---

### ENUM_LICENSE_TYPE
```mql5
ENUM_LICENSE_TYPE
```

---

### LICENSE_FREE
```mql5
LICENSE_FREE
```

---

### LICENSE_DEMO
```mql5
LICENSE_DEMO
```

---

### LICENSE_TIME
```mql5
LICENSE_TIME
```

---

### ENUM_SYMBOL_INFO_INTEGER
```mql5
ENUM_SYMBOL_INFO_INTEGER
```

---

### SYMBOL_SUBSCRIPTION_DELAY
```mql5
SYMBOL_SUBSCRIPTION_DELAY
```

---

### SYMBOL_SECTOR
```mql5
SYMBOL_SECTOR
```

---

### SYMBOL_INDUSTRY
```mql5
SYMBOL_INDUSTRY
```

---

### SYMBOL_CUSTOM
```mql5
SYMBOL_CUSTOM
```

---

### SYMBOL_BACKGROUND_COLOR
```mql5
SYMBOL_BACKGROUND_COLOR
```

---

### SYMBOL_CHART_MODE
```mql5
SYMBOL_CHART_MODE
```

---

### SYMBOL_SELECT
```mql5
SYMBOL_SELECT
```

---

### SYMBOL_VISIBLE
```mql5
SYMBOL_VISIBLE
```

---

### SYMBOL_SESSION_DEALS
```mql5
SYMBOL_SESSION_DEALS
```

---

### SYMBOL_SESSION_BUY_ORDERS
```mql5
SYMBOL_SESSION_BUY_ORDERS
```

---

### SYMBOL_SESSION_SELL_ORDERS
```mql5
SYMBOL_SESSION_SELL_ORDERS
```

---

### SYMBOL_VOLUME
```mql5
SYMBOL_VOLUME
```

---

### SYMBOL_VOLUMEHIGH
```mql5
SYMBOL_VOLUMEHIGH
```

---

### SYMBOL_VOLUMELOW
```mql5
SYMBOL_VOLUMELOW
```

---

### SYMBOL_TIME
```mql5
SYMBOL_TIME
```

---

### SYMBOL_TIME_MSC
```mql5
SYMBOL_TIME_MSC
```

---

### SYMBOL_DIGITS
```mql5
SYMBOL_DIGITS
```

---

### SYMBOL_SPREAD_FLOAT
```mql5
SYMBOL_SPREAD_FLOAT
```

---

### SYMBOL_SPREAD
```mql5
SYMBOL_SPREAD
```

---

### SYMBOL_TICKS_BOOKDEPTH
```mql5
SYMBOL_TICKS_BOOKDEPTH
```

---

### SYMBOL_TRADE_CALC_MODE
```mql5
SYMBOL_TRADE_CALC_MODE
```

---

### SYMBOL_TRADE_MODE
```mql5
SYMBOL_TRADE_MODE
```

---

### SYMBOL_START_TIME
```mql5
SYMBOL_START_TIME
```

---

### SYMBOL_EXPIRATION_TIME
```mql5
SYMBOL_EXPIRATION_TIME
```

---

### SYMBOL_TRADE_STOPS_LEVEL
```mql5
SYMBOL_TRADE_STOPS_LEVEL
```

---

### SYMBOL_TRADE_FREEZE_LEVEL
```mql5
SYMBOL_TRADE_FREEZE_LEVEL
```

---

### SYMBOL_TRADE_EXEMODE
```mql5
SYMBOL_TRADE_EXEMODE
```

---

### SYMBOL_SWAP_MODE
```mql5
SYMBOL_SWAP_MODE
```

---

### SYMBOL_SWAP_ROLLOVER3DAYS
```mql5
SYMBOL_SWAP_ROLLOVER3DAYS
```

---

### SYMBOL_MARGIN_HEDGED_USE_LEG
```mql5
SYMBOL_MARGIN_HEDGED_USE_LEG
```

---

### SYMBOL_EXPIRATION_MODE
```mql5
SYMBOL_EXPIRATION_MODE
```

---

### SYMBOL_FILLING_MODE
```mql5
SYMBOL_FILLING_MODE
```

---

### SYMBOL_ORDER_MODE
```mql5
SYMBOL_ORDER_MODE
```

---

### SYMBOL_ORDER_GTC_MODE
```mql5
SYMBOL_ORDER_GTC_MODE
```

---

### SYMBOL_OPTION_MODE
```mql5
SYMBOL_OPTION_MODE
```

---

### SYMBOL_OPTION_RIGHT
```mql5
SYMBOL_OPTION_RIGHT
```

---

### ENUM_SYMBOL_INFO_DOUBLE
```mql5
ENUM_SYMBOL_INFO_DOUBLE
```

---

### SYMBOL_BID
```mql5
SYMBOL_BID
```

---

### SYMBOL_BIDHIGH
```mql5
SYMBOL_BIDHIGH
```

---

### SYMBOL_BIDLOW
```mql5
SYMBOL_BIDLOW
```

---

### SYMBOL_ASK
```mql5
SYMBOL_ASK
```

---

### SYMBOL_ASKHIGH
```mql5
SYMBOL_ASKHIGH
```

---

### SYMBOL_ASKLOW
```mql5
SYMBOL_ASKLOW
```

---

### SYMBOL_LAST
```mql5
SYMBOL_LAST
```

---

### SYMBOL_LASTHIGH
```mql5
SYMBOL_LASTHIGH
```

---

### SYMBOL_LASTLOW
```mql5
SYMBOL_LASTLOW
```

---

### SYMBOL_VOLUME_REAL
```mql5
SYMBOL_VOLUME_REAL
```

---

### SYMBOL_VOLUMEHIGH_REAL
```mql5
SYMBOL_VOLUMEHIGH_REAL
```

---

### SYMBOL_VOLUMELOW_REAL
```mql5
SYMBOL_VOLUMELOW_REAL
```

---

### SYMBOL_OPTION_STRIKE
```mql5
SYMBOL_OPTION_STRIKE
```

---

### SYMBOL_POINT
```mql5
SYMBOL_POINT
```

---

### SYMBOL_TRADE_TICK_VALUE
```mql5
SYMBOL_TRADE_TICK_VALUE
```

---

### SYMBOL_TRADE_TICK_VALUE_PROFIT
```mql5
SYMBOL_TRADE_TICK_VALUE_PROFIT
```

---

### SYMBOL_TRADE_TICK_VALUE_LOSS
```mql5
SYMBOL_TRADE_TICK_VALUE_LOSS
```

---

### SYMBOL_TRADE_TICK_SIZE
```mql5
SYMBOL_TRADE_TICK_SIZE
```

---

### SYMBOL_TRADE_CONTRACT_SIZE
```mql5
SYMBOL_TRADE_CONTRACT_SIZE
```

---

### SYMBOL_TRADE_ACCRUED_INTEREST
```mql5
SYMBOL_TRADE_ACCRUED_INTEREST
```

---

### SYMBOL_TRADE_FACE_VALUE
```mql5
SYMBOL_TRADE_FACE_VALUE
```

---

### SYMBOL_TRADE_LIQUIDITY_RATE
```mql5
SYMBOL_TRADE_LIQUIDITY_RATE
```

---

### SYMBOL_VOLUME_MIN
```mql5
SYMBOL_VOLUME_MIN
```

---

### SYMBOL_VOLUME_MAX
```mql5
SYMBOL_VOLUME_MAX
```

---

### SYMBOL_VOLUME_STEP
```mql5
SYMBOL_VOLUME_STEP
```

---

### SYMBOL_VOLUME_LIMIT
```mql5
SYMBOL_VOLUME_LIMIT
```

---

### SYMBOL_SWAP_LONG
```mql5
SYMBOL_SWAP_LONG
```

---

### SYMBOL_SWAP_SHORT
```mql5
SYMBOL_SWAP_SHORT
```

---

### SYMBOL_MARGIN_INITIAL
```mql5
SYMBOL_MARGIN_INITIAL
```

---

### SYMBOL_MARGIN_MAINTENANCE
```mql5
SYMBOL_MARGIN_MAINTENANCE
```

---

### SYMBOL_SESSION_VOLUME
```mql5
SYMBOL_SESSION_VOLUME
```

---

### SYMBOL_SESSION_TURNOVER
```mql5
SYMBOL_SESSION_TURNOVER
```

---

### SYMBOL_SESSION_INTEREST
```mql5
SYMBOL_SESSION_INTEREST
```

---

### SYMBOL_SESSION_BUY_ORDERS_VOLUME
```mql5
SYMBOL_SESSION_BUY_ORDERS_VOLUME
```

---

### SYMBOL_SESSION_SELL_ORDERS_VOLUME
```mql5
SYMBOL_SESSION_SELL_ORDERS_VOLUME
```

---

### SYMBOL_SESSION_OPEN
```mql5
SYMBOL_SESSION_OPEN
```

---

### SYMBOL_SESSION_CLOSE
```mql5
SYMBOL_SESSION_CLOSE
```

---

### SYMBOL_SESSION_AW
```mql5
SYMBOL_SESSION_AW
```

---

### SYMBOL_SESSION_PRICE_SETTLEMENT
```mql5
SYMBOL_SESSION_PRICE_SETTLEMENT
```

---

### SYMBOL_SESSION_PRICE_LIMIT_MIN
```mql5
SYMBOL_SESSION_PRICE_LIMIT_MIN
```

---

### SYMBOL_SESSION_PRICE_LIMIT_MAX
```mql5
SYMBOL_SESSION_PRICE_LIMIT_MAX
```

---

### SYMBOL_MARGIN_HEDGED
```mql5
SYMBOL_MARGIN_HEDGED
```

---

### SYMBOL_PRICE_CHANGE
```mql5
SYMBOL_PRICE_CHANGE
```

---

### SYMBOL_PRICE_VOLATILITY
```mql5
SYMBOL_PRICE_VOLATILITY
```

---

### SYMBOL_PRICE_THEORETICAL
```mql5
SYMBOL_PRICE_THEORETICAL
```

---

### SYMBOL_PRICE_DELTA
```mql5
SYMBOL_PRICE_DELTA
```

---

### SYMBOL_PRICE_THETA
```mql5
SYMBOL_PRICE_THETA
```

---

### SYMBOL_PRICE_GAMMA
```mql5
SYMBOL_PRICE_GAMMA
```

---

### SYMBOL_PRICE_VEGA
```mql5
SYMBOL_PRICE_VEGA
```

---

### SYMBOL_PRICE_RHO
```mql5
SYMBOL_PRICE_RHO
```

---

### SYMBOL_PRICE_OMEGA
```mql5
SYMBOL_PRICE_OMEGA
```

---

### SYMBOL_PRICE_SENSITIVITY
```mql5
SYMBOL_PRICE_SENSITIVITY
```

---

### ENUM_SYMBOL_INFO_STRING
```mql5
ENUM_SYMBOL_INFO_STRING
```

---

### SYMBOL_BASIS
```mql5
SYMBOL_BASIS
```

---

### SYMBOL_CATEGORY
```mql5
SYMBOL_CATEGORY
```

---

### SYMBOL_COUNTRY
```mql5
SYMBOL_COUNTRY
```

---

### SYMBOL_SECTOR_NAME
```mql5
SYMBOL_SECTOR_NAME
```

---

### SYMBOL_INDUSTRY_NAME
```mql5
SYMBOL_INDUSTRY_NAME
```

---

### SYMBOL_CURRENCY_BASE
```mql5
SYMBOL_CURRENCY_BASE
```

---

### SYMBOL_CURRENCY_PROFIT
```mql5
SYMBOL_CURRENCY_PROFIT
```

---

### SYMBOL_CURRENCY_MARGIN
```mql5
SYMBOL_CURRENCY_MARGIN
```

---

### SYMBOL_BANK
```mql5
SYMBOL_BANK
```

---

### SYMBOL_DESCRIPTION
```mql5
SYMBOL_DESCRIPTION
```

---

### SYMBOL_EXCHANGE
```mql5
SYMBOL_EXCHANGE
```

---

### SYMBOL_FORMULA
```mql5
SYMBOL_FORMULA
```

---

### SYMBOL_ISIN
```mql5
SYMBOL_ISIN
```

---

### SYMBOL_PAGE
```mql5
SYMBOL_PAGE
```

---

### SYMBOL_PATH
```mql5
SYMBOL_PATH
```

---

### ENUM_SYMBOL_CHART_MODE
```mql5
ENUM_SYMBOL_CHART_MODE
```

---

### SYMBOL_CHART_MODE_BID
```mql5
SYMBOL_CHART_MODE_BID
```

---

### SYMBOL_CHART_MODE_LAST
```mql5
SYMBOL_CHART_MODE_LAST
```

---

### ENUM_SYMBOL_ORDER_GTC_MODE
```mql5
ENUM_SYMBOL_ORDER_GTC_MODE
```

---

### SYMBOL_ORDERS_GTC
```mql5
SYMBOL_ORDERS_GTC
```

---

### SYMBOL_ORDERS_DAILY
```mql5
SYMBOL_ORDERS_DAILY
```

---

### SYMBOL_ORDERS_DAILY_EXCLUDING_STOPS
```mql5
SYMBOL_ORDERS_DAILY_EXCLUDING_STOPS
```

---

### ENUM_SYMBOL_CALC_MODE
```mql5
ENUM_SYMBOL_CALC_MODE
```

---

### SYMBOL_CALC_MODE_FOREX
```mql5
SYMBOL_CALC_MODE_FOREX
```

---

### SYMBOL_CALC_MODE_FOREX_NO_LEVERAGE
```mql5
SYMBOL_CALC_MODE_FOREX_NO_LEVERAGE
```

---

### SYMBOL_CALC_MODE_FUTURES
```mql5
SYMBOL_CALC_MODE_FUTURES
```

---

### SYMBOL_CALC_MODE_CFD
```mql5
SYMBOL_CALC_MODE_CFD
```

---

### SYMBOL_CALC_MODE_CFDINDEX
```mql5
SYMBOL_CALC_MODE_CFDINDEX
```

---

### SYMBOL_CALC_MODE_CFDLEVERAGE
```mql5
SYMBOL_CALC_MODE_CFDLEVERAGE
```

---

### SYMBOL_CALC_MODE_EXCH_STOCKS
```mql5
SYMBOL_CALC_MODE_EXCH_STOCKS
```

---

### SYMBOL_CALC_MODE_EXCH_FUTURES
```mql5
SYMBOL_CALC_MODE_EXCH_FUTURES
```

---

### SYMBOL_CALC_MODE_EXCH_FUTURES_FORTS
```mql5
SYMBOL_CALC_MODE_EXCH_FUTURES_FORTS
```

---

### SYMBOL_CALC_MODE_EXCH_BONDS
```mql5
SYMBOL_CALC_MODE_EXCH_BONDS
```

---

### SYMBOL_CALC_MODE_EXCH_STOCKS_MOEX
```mql5
SYMBOL_CALC_MODE_EXCH_STOCKS_MOEX
```

---

### SYMBOL_CALC_MODE_EXCH_BONDS_MOEX
```mql5
SYMBOL_CALC_MODE_EXCH_BONDS_MOEX
```

---

### SYMBOL_CALC_MODE_SERV_COLLATERAL
```mql5
SYMBOL_CALC_MODE_SERV_COLLATERAL
```

---

### ENUM_SYMBOL_TRADE_MODE
```mql5
ENUM_SYMBOL_TRADE_MODE
```

---

### SYMBOL_TRADE_MODE_DISABLED
```mql5
SYMBOL_TRADE_MODE_DISABLED
```

---

### SYMBOL_TRADE_MODE_LONGONLY
```mql5
SYMBOL_TRADE_MODE_LONGONLY
```

---

### SYMBOL_TRADE_MODE_SHORTONLY
```mql5
SYMBOL_TRADE_MODE_SHORTONLY
```

---

### SYMBOL_TRADE_MODE_CLOSEONLY
```mql5
SYMBOL_TRADE_MODE_CLOSEONLY
```

---

### SYMBOL_TRADE_MODE_FULL
```mql5
SYMBOL_TRADE_MODE_FULL
```

---

### ENUM_SYMBOL_TRADE_EXECUTION
```mql5
ENUM_SYMBOL_TRADE_EXECUTION
```

---

### SYMBOL_TRADE_EXECUTION_REQUEST
```mql5
SYMBOL_TRADE_EXECUTION_REQUEST
```

---

### SYMBOL_TRADE_EXECUTION_INSTANT
```mql5
SYMBOL_TRADE_EXECUTION_INSTANT
```

---

### SYMBOL_TRADE_EXECUTION_MARKET
```mql5
SYMBOL_TRADE_EXECUTION_MARKET
```

---

### SYMBOL_TRADE_EXECUTION_EXCHANGE
```mql5
SYMBOL_TRADE_EXECUTION_EXCHANGE
```

---

### ENUM_SYMBOL_SWAP_MODE
```mql5
ENUM_SYMBOL_SWAP_MODE
```

---

### SYMBOL_SWAP_MODE_DISABLED
```mql5
SYMBOL_SWAP_MODE_DISABLED
```

---

### SYMBOL_SWAP_MODE_POINTS
```mql5
SYMBOL_SWAP_MODE_POINTS
```

---

### SYMBOL_SWAP_MODE_CURRENCY_SYMBOL
```mql5
SYMBOL_SWAP_MODE_CURRENCY_SYMBOL
```

---

### SYMBOL_SWAP_MODE_CURRENCY_MARGIN
```mql5
SYMBOL_SWAP_MODE_CURRENCY_MARGIN
```

---

### SYMBOL_SWAP_MODE_CURRENCY_DEPOSIT
```mql5
SYMBOL_SWAP_MODE_CURRENCY_DEPOSIT
```

---

### SYMBOL_SWAP_MODE_INTEREST_CURRENT
```mql5
SYMBOL_SWAP_MODE_INTEREST_CURRENT
```

---

### SYMBOL_SWAP_MODE_INTEREST_OPEN
```mql5
SYMBOL_SWAP_MODE_INTEREST_OPEN
```

---

### SYMBOL_SWAP_MODE_REOPEN_CURRENT
```mql5
SYMBOL_SWAP_MODE_REOPEN_CURRENT
```

---

### SYMBOL_SWAP_MODE_REOPEN_BID
```mql5
SYMBOL_SWAP_MODE_REOPEN_BID
```

---

### ENUM_DAY_OF_WEEK
```mql5
ENUM_DAY_OF_WEEK
```

---

### SUNDAY
```mql5
SUNDAY
```

---

### MONDAY
```mql5
MONDAY
```

---

### TUESDAY
```mql5
TUESDAY
```

---

### WEDNESDAY
```mql5
WEDNESDAY
```

---

### THURSDAY
```mql5
THURSDAY
```

---

### FRIDAY
```mql5
FRIDAY
```

---

### SATURDAY
```mql5
SATURDAY
```

---

### ENUM_SYMBOL_OPTION_RIGHT
```mql5
ENUM_SYMBOL_OPTION_RIGHT
```

---

### SYMBOL_OPTION_RIGHT_CALL
```mql5
SYMBOL_OPTION_RIGHT_CALL
```

---

### SYMBOL_OPTION_RIGHT_PUT
```mql5
SYMBOL_OPTION_RIGHT_PUT
```

---

### ENUM_SYMBOL_OPTION_MODE
```mql5
ENUM_SYMBOL_OPTION_MODE
```

---

### SYMBOL_OPTION_MODE_EUROPEAN
```mql5
SYMBOL_OPTION_MODE_EUROPEAN
```

---

### SYMBOL_OPTION_MODE_AMERICAN
```mql5
SYMBOL_OPTION_MODE_AMERICAN
```

---

### ENUM_SYMBOL_SECTOR
```mql5
ENUM_SYMBOL_SECTOR
```

---

### SECTOR_UNDEFINED
```mql5
SECTOR_UNDEFINED
```

---

### SECTOR_BASIC_MATERIALS
```mql5
SECTOR_BASIC_MATERIALS
```

---

### SECTOR_COMMUNICATION_SERVICES
```mql5
SECTOR_COMMUNICATION_SERVICES
```

---

### SECTOR_CONSUMER_CYCLICAL
```mql5
SECTOR_CONSUMER_CYCLICAL
```

---

### SECTOR_CONSUMER_DEFENSIVE
```mql5
SECTOR_CONSUMER_DEFENSIVE
```

---

### SECTOR_CURRENCY
```mql5
SECTOR_CURRENCY
```

---

### SECTOR_CURRENCY_CRYPTO
```mql5
SECTOR_CURRENCY_CRYPTO
```

---

### SECTOR_ENERGY
```mql5
SECTOR_ENERGY
```

---

### SECTOR_FINANCIAL
```mql5
SECTOR_FINANCIAL
```

---

### SECTOR_HEALTHCARE
```mql5
SECTOR_HEALTHCARE
```

---

### SECTOR_INDUSTRIALS
```mql5
SECTOR_INDUSTRIALS
```

---

### SECTOR_REAL_ESTATE
```mql5
SECTOR_REAL_ESTATE
```

---

### SECTOR_TECHNOLOGY
```mql5
SECTOR_TECHNOLOGY
```

---

### SECTOR_UTILITIES
```mql5
SECTOR_UTILITIES
```

---

### ENUM_SYMBOL_INDUSTRY
```mql5
ENUM_SYMBOL_INDUSTRY
```

---

### INDUSTRY_UNDEFINED
```mql5
INDUSTRY_UNDEFINED
```

---

### INDUSTRY_AGRICULTURAL_INPUTS
```mql5
INDUSTRY_AGRICULTURAL_INPUTS
```

---

### INDUSTRY_ALUMINIUM
```mql5
INDUSTRY_ALUMINIUM
```

---

### INDUSTRY_BUILDING_MATERIALS
```mql5
INDUSTRY_BUILDING_MATERIALS
```

---

### INDUSTRY_CHEMICALS
```mql5
INDUSTRY_CHEMICALS
```

---

### INDUSTRY_COKING_COAL
```mql5
INDUSTRY_COKING_COAL
```

---

### INDUSTRY_COPPER
```mql5
INDUSTRY_COPPER
```

---

### INDUSTRY_GOLD
```mql5
INDUSTRY_GOLD
```

---

### INDUSTRY_LUMBER_WOOD
```mql5
INDUSTRY_LUMBER_WOOD
```

---

### INDUSTRY_INDUSTRIAL_METALS
```mql5
INDUSTRY_INDUSTRIAL_METALS
```

---

### INDUSTRY_PRECIOUS_METALS
```mql5
INDUSTRY_PRECIOUS_METALS
```

---

### INDUSTRY_PAPER
```mql5
INDUSTRY_PAPER
```

---

### INDUSTRY_SILVER
```mql5
INDUSTRY_SILVER
```

---

### INDUSTRY_SPECIALTY_CHEMICALS
```mql5
INDUSTRY_SPECIALTY_CHEMICALS
```

---

### INDUSTRY_STEEL
```mql5
INDUSTRY_STEEL
```

---

### INDUSTRY_ADVERTISING
```mql5
INDUSTRY_ADVERTISING
```

---

### INDUSTRY_BROADCASTING
```mql5
INDUSTRY_BROADCASTING
```

---

### INDUSTRY_GAMING_MULTIMEDIA
```mql5
INDUSTRY_GAMING_MULTIMEDIA
```

---

### INDUSTRY_ENTERTAINMENT
```mql5
INDUSTRY_ENTERTAINMENT
```

---

### INDUSTRY_INTERNET_CONTENT
```mql5
INDUSTRY_INTERNET_CONTENT
```

---

### INDUSTRY_PUBLISHING
```mql5
INDUSTRY_PUBLISHING
```

---

### INDUSTRY_TELECOM
```mql5
INDUSTRY_TELECOM
```

---

### INDUSTRY_APPAREL_MANUFACTURING
```mql5
INDUSTRY_APPAREL_MANUFACTURING
```

---

### INDUSTRY_APPAREL_RETAIL
```mql5
INDUSTRY_APPAREL_RETAIL
```

---

### INDUSTRY_AUTO_MANUFACTURERS
```mql5
INDUSTRY_AUTO_MANUFACTURERS
```

---

### INDUSTRY_AUTO_PARTS
```mql5
INDUSTRY_AUTO_PARTS
```

---

### INDUSTRY_AUTO_DEALERSHIP
```mql5
INDUSTRY_AUTO_DEALERSHIP
```

---

### INDUSTRY_DEPARTMENT_STORES
```mql5
INDUSTRY_DEPARTMENT_STORES
```

---

### INDUSTRY_FOOTWEAR_ACCESSORIES
```mql5
INDUSTRY_FOOTWEAR_ACCESSORIES
```

---

### INDUSTRY_FURNISHINGS
```mql5
INDUSTRY_FURNISHINGS
```

---

### INDUSTRY_GAMBLING
```mql5
INDUSTRY_GAMBLING
```

---

### INDUSTRY_HOME_IMPROV_RETAIL
```mql5
INDUSTRY_HOME_IMPROV_RETAIL
```

---

### INDUSTRY_INTERNET_RETAIL
```mql5
INDUSTRY_INTERNET_RETAIL
```

---

### INDUSTRY_LEISURE
```mql5
INDUSTRY_LEISURE
```

---

### INDUSTRY_LODGING
```mql5
INDUSTRY_LODGING
```

---

### INDUSTRY_LUXURY_GOODS
```mql5
INDUSTRY_LUXURY_GOODS
```

---

### INDUSTRY_PACKAGING_CONTAINERS
```mql5
INDUSTRY_PACKAGING_CONTAINERS
```

---

### INDUSTRY_PERSONAL_SERVICES
```mql5
INDUSTRY_PERSONAL_SERVICES
```

---

### INDUSTRY_RECREATIONAL_VEHICLES
```mql5
INDUSTRY_RECREATIONAL_VEHICLES
```

---

### INDUSTRY_RESIDENT_CONSTRUCTION
```mql5
INDUSTRY_RESIDENT_CONSTRUCTION
```

---

### INDUSTRY_RESORTS_CASINOS
```mql5
INDUSTRY_RESORTS_CASINOS
```

---

### INDUSTRY_RESTAURANTS
```mql5
INDUSTRY_RESTAURANTS
```

---

### INDUSTRY_SPECIALTY_RETAIL
```mql5
INDUSTRY_SPECIALTY_RETAIL
```

---

### INDUSTRY_TEXTILE_MANUFACTURING
```mql5
INDUSTRY_TEXTILE_MANUFACTURING
```

---

### INDUSTRY_TRAVEL_SERVICES
```mql5
INDUSTRY_TRAVEL_SERVICES
```

---

### INDUSTRY_BEVERAGES_BREWERS
```mql5
INDUSTRY_BEVERAGES_BREWERS
```

---

### INDUSTRY_BEVERAGES_NON_ALCO
```mql5
INDUSTRY_BEVERAGES_NON_ALCO
```

---

### INDUSTRY_BEVERAGES_WINERIES
```mql5
INDUSTRY_BEVERAGES_WINERIES
```

---

### INDUSTRY_CONFECTIONERS
```mql5
INDUSTRY_CONFECTIONERS
```

---

### INDUSTRY_DISCOUNT_STORES
```mql5
INDUSTRY_DISCOUNT_STORES
```

---

### INDUSTRY_EDUCATION_TRAINIG
```mql5
INDUSTRY_EDUCATION_TRAINIG
```

---

### INDUSTRY_FARM_PRODUCTS
```mql5
INDUSTRY_FARM_PRODUCTS
```

---

### INDUSTRY_FOOD_DISTRIBUTION
```mql5
INDUSTRY_FOOD_DISTRIBUTION
```

---

### INDUSTRY_GROCERY_STORES
```mql5
INDUSTRY_GROCERY_STORES
```

---

### INDUSTRY_HOUSEHOLD_PRODUCTS
```mql5
INDUSTRY_HOUSEHOLD_PRODUCTS
```

---

### INDUSTRY_PACKAGED_FOODS
```mql5
INDUSTRY_PACKAGED_FOODS
```

---

### INDUSTRY_TOBACCO
```mql5
INDUSTRY_TOBACCO
```

---

### INDUSTRY_OIL_GAS_DRILLING
```mql5
INDUSTRY_OIL_GAS_DRILLING
```

---

### INDUSTRY_OIL_GAS_EP
```mql5
INDUSTRY_OIL_GAS_EP
```

---

### INDUSTRY_OIL_GAS_EQUIPMENT
```mql5
INDUSTRY_OIL_GAS_EQUIPMENT
```

---

### INDUSTRY_OIL_GAS_INTEGRATED
```mql5
INDUSTRY_OIL_GAS_INTEGRATED
```

---

### INDUSTRY_OIL_GAS_MIDSTREAM
```mql5
INDUSTRY_OIL_GAS_MIDSTREAM
```

---

### INDUSTRY_OIL_GAS_REFINING
```mql5
INDUSTRY_OIL_GAS_REFINING
```

---

### INDUSTRY_THERMAL_COAL
```mql5
INDUSTRY_THERMAL_COAL
```

---

### INDUSTRY_URANIUM
```mql5
INDUSTRY_URANIUM
```

---

### INDUSTRY_EXCHANGE_TRADED_FUND
```mql5
INDUSTRY_EXCHANGE_TRADED_FUND
```

---

### INDUSTRY_ASSETS_MANAGEMENT
```mql5
INDUSTRY_ASSETS_MANAGEMENT
```

---

### INDUSTRY_BANKS_DIVERSIFIED
```mql5
INDUSTRY_BANKS_DIVERSIFIED
```

---

### INDUSTRY_BANKS_REGIONAL
```mql5
INDUSTRY_BANKS_REGIONAL
```

---

### INDUSTRY_CAPITAL_MARKETS
```mql5
INDUSTRY_CAPITAL_MARKETS
```

---

### INDUSTRY_CLOSE_END_FUND_DEBT
```mql5
INDUSTRY_CLOSE_END_FUND_DEBT
```

---

### INDUSTRY_CLOSE_END_FUND_EQUITY
```mql5
INDUSTRY_CLOSE_END_FUND_EQUITY
```

---

### INDUSTRY_CLOSE_END_FUND_FOREIGN
```mql5
INDUSTRY_CLOSE_END_FUND_FOREIGN
```

---

### INDUSTRY_CREDIT_SERVICES
```mql5
INDUSTRY_CREDIT_SERVICES
```

---

### INDUSTRY_FINANCIAL_CONGLOMERATE
```mql5
INDUSTRY_FINANCIAL_CONGLOMERATE
```

---

### INDUSTRY_FINANCIAL_DATA_EXCHANGE
```mql5
INDUSTRY_FINANCIAL_DATA_EXCHANGE
```

---

### INDUSTRY_INSURANCE_BROKERS
```mql5
INDUSTRY_INSURANCE_BROKERS
```

---

### INDUSTRY_INSURANCE_DIVERSIFIED
```mql5
INDUSTRY_INSURANCE_DIVERSIFIED
```

---

### INDUSTRY_INSURANCE_LIFE
```mql5
INDUSTRY_INSURANCE_LIFE
```

---

### INDUSTRY_INSURANCE_PROPERTY
```mql5
INDUSTRY_INSURANCE_PROPERTY
```

---

### INDUSTRY_INSURANCE_REINSURANCE
```mql5
INDUSTRY_INSURANCE_REINSURANCE
```

---

### INDUSTRY_INSURANCE_SPECIALTY
```mql5
INDUSTRY_INSURANCE_SPECIALTY
```

---

### INDUSTRY_MORTGAGE_FINANCE
```mql5
INDUSTRY_MORTGAGE_FINANCE
```

---

### INDUSTRY_SHELL_COMPANIES
```mql5
INDUSTRY_SHELL_COMPANIES
```

---

### INDUSTRY_BIOTECHNOLOGY
```mql5
INDUSTRY_BIOTECHNOLOGY
```

---

### INDUSTRY_DIAGNOSTICS_RESEARCH
```mql5
INDUSTRY_DIAGNOSTICS_RESEARCH
```

---

### INDUSTRY_DRUGS_MANUFACTURERS
```mql5
INDUSTRY_DRUGS_MANUFACTURERS
```

---

### INDUSTRY_DRUGS_MANUFACTURERS_SPEC
```mql5
INDUSTRY_DRUGS_MANUFACTURERS_SPEC
```

---

### INDUSTRY_HEALTHCARE_PLANS
```mql5
INDUSTRY_HEALTHCARE_PLANS
```

---

### INDUSTRY_HEALTH_INFORMATION
```mql5
INDUSTRY_HEALTH_INFORMATION
```

---

### INDUSTRY_MEDICAL_FACILITIES
```mql5
INDUSTRY_MEDICAL_FACILITIES
```

---

### INDUSTRY_MEDICAL_DEVICES
```mql5
INDUSTRY_MEDICAL_DEVICES
```

---

### INDUSTRY_MEDICAL_DISTRIBUTION
```mql5
INDUSTRY_MEDICAL_DISTRIBUTION
```

---

### INDUSTRY_MEDICAL_INSTRUMENTS
```mql5
INDUSTRY_MEDICAL_INSTRUMENTS
```

---

### INDUSTRY_PHARM_RETAILERS
```mql5
INDUSTRY_PHARM_RETAILERS
```

---

### INDUSTRY_AEROSPACE_DEFENSE
```mql5
INDUSTRY_AEROSPACE_DEFENSE
```

---

### INDUSTRY_AIRLINES
```mql5
INDUSTRY_AIRLINES
```

---

### INDUSTRY_AIRPORTS_SERVICES
```mql5
INDUSTRY_AIRPORTS_SERVICES
```

---

### INDUSTRY_BUILDING_PRODUCTS
```mql5
INDUSTRY_BUILDING_PRODUCTS
```

---

### INDUSTRY_BUSINESS_EQUIPMENT
```mql5
INDUSTRY_BUSINESS_EQUIPMENT
```

---

### INDUSTRY_CONGLOMERATES
```mql5
INDUSTRY_CONGLOMERATES
```

---

### INDUSTRY_CONSULTING_SERVICES
```mql5
INDUSTRY_CONSULTING_SERVICES
```

---

### INDUSTRY_ELECTRICAL_EQUIPMENT
```mql5
INDUSTRY_ELECTRICAL_EQUIPMENT
```

---

### INDUSTRY_ENGINEERING_CONSTRUCTION
```mql5
INDUSTRY_ENGINEERING_CONSTRUCTION
```

---

### INDUSTRY_FARM_HEAVY_MACHINERY
```mql5
INDUSTRY_FARM_HEAVY_MACHINERY
```

---

### INDUSTRY_INDUSTRIAL_DISTRIBUTION
```mql5
INDUSTRY_INDUSTRIAL_DISTRIBUTION
```

---

### INDUSTRY_INFRASTRUCTURE_OPERATIONS
```mql5
INDUSTRY_INFRASTRUCTURE_OPERATIONS
```

---

### INDUSTRY_FREIGHT_LOGISTICS
```mql5
INDUSTRY_FREIGHT_LOGISTICS
```

---

### INDUSTRY_MARINE_SHIPPING
```mql5
INDUSTRY_MARINE_SHIPPING
```

---

### INDUSTRY_METAL_FABRICATION
```mql5
INDUSTRY_METAL_FABRICATION
```

---

### INDUSTRY_POLLUTION_CONTROL
```mql5
INDUSTRY_POLLUTION_CONTROL
```

---

### INDUSTRY_RAILROADS
```mql5
INDUSTRY_RAILROADS
```

---

### INDUSTRY_RENTAL_LEASING
```mql5
INDUSTRY_RENTAL_LEASING
```

---

### INDUSTRY_SECURITY_PROTECTION
```mql5
INDUSTRY_SECURITY_PROTECTION
```

---

### INDUSTRY_SPEALITY_BUSINESS_SERVICES
```mql5
INDUSTRY_SPEALITY_BUSINESS_SERVICES
```

---

### INDUSTRY_SPEALITY_MACHINERY
```mql5
INDUSTRY_SPEALITY_MACHINERY
```

---

### INDUSTRY_STUFFING_EMPLOYMENT
```mql5
INDUSTRY_STUFFING_EMPLOYMENT
```

---

### INDUSTRY_TOOLS_ACCESSORIES
```mql5
INDUSTRY_TOOLS_ACCESSORIES
```

---

### INDUSTRY_TRUCKING
```mql5
INDUSTRY_TRUCKING
```

---

### INDUSTRY_WASTE_MANAGEMENT
```mql5
INDUSTRY_WASTE_MANAGEMENT
```

---

### INDUSTRY_REAL_ESTATE_DEVELOPMENT
```mql5
INDUSTRY_REAL_ESTATE_DEVELOPMENT
```

---

### INDUSTRY_REAL_ESTATE_DIVERSIFIED
```mql5
INDUSTRY_REAL_ESTATE_DIVERSIFIED
```

---

### INDUSTRY_REAL_ESTATE_SERVICES
```mql5
INDUSTRY_REAL_ESTATE_SERVICES
```

---

### INDUSTRY_REIT_DIVERSIFIED
```mql5
INDUSTRY_REIT_DIVERSIFIED
```

---

### INDUSTRY_REIT_HEALTCARE
```mql5
INDUSTRY_REIT_HEALTCARE
```

---

### INDUSTRY_REIT_HOTEL_MOTEL
```mql5
INDUSTRY_REIT_HOTEL_MOTEL
```

---

### INDUSTRY_REIT_INDUSTRIAL
```mql5
INDUSTRY_REIT_INDUSTRIAL
```

---

### INDUSTRY_REIT_MORTAGE
```mql5
INDUSTRY_REIT_MORTAGE
```

---

### INDUSTRY_REIT_OFFICE
```mql5
INDUSTRY_REIT_OFFICE
```

---

### INDUSTRY_REIT_RESIDENTAL
```mql5
INDUSTRY_REIT_RESIDENTAL
```

---

### INDUSTRY_REIT_RETAIL
```mql5
INDUSTRY_REIT_RETAIL
```

---

### INDUSTRY_REIT_SPECIALITY
```mql5
INDUSTRY_REIT_SPECIALITY
```

---

### INDUSTRY_COMMUNICATION_EQUIPMENT
```mql5
INDUSTRY_COMMUNICATION_EQUIPMENT
```

---

### INDUSTRY_COMPUTER_HARDWARE
```mql5
INDUSTRY_COMPUTER_HARDWARE
```

---

### INDUSTRY_CONSUMER_ELECTRONICS
```mql5
INDUSTRY_CONSUMER_ELECTRONICS
```

---

### INDUSTRY_ELECTRONIC_COMPONENTS
```mql5
INDUSTRY_ELECTRONIC_COMPONENTS
```

---

### INDUSTRY_ELECTRONIC_DISTRIBUTION
```mql5
INDUSTRY_ELECTRONIC_DISTRIBUTION
```

---

### INDUSTRY_IT_SERVICES
```mql5
INDUSTRY_IT_SERVICES
```

---

### INDUSTRY_SCIENTIFIC_INSTRUMENTS
```mql5
INDUSTRY_SCIENTIFIC_INSTRUMENTS
```

---

### INDUSTRY_SEMICONDUCTOR_EQUIPMENT
```mql5
INDUSTRY_SEMICONDUCTOR_EQUIPMENT
```

---

### INDUSTRY_SEMICONDUCTORS
```mql5
INDUSTRY_SEMICONDUCTORS
```

---

### INDUSTRY_SOFTWARE_APPLICATION
```mql5
INDUSTRY_SOFTWARE_APPLICATION
```

---

### INDUSTRY_SOFTWARE_INFRASTRUCTURE
```mql5
INDUSTRY_SOFTWARE_INFRASTRUCTURE
```

---

### INDUSTRY_SOLAR
```mql5
INDUSTRY_SOLAR
```

---

### INDUSTRY_UTILITIES_DIVERSIFIED
```mql5
INDUSTRY_UTILITIES_DIVERSIFIED
```

---

### INDUSTRY_UTILITIES_POWERPRODUCERS
```mql5
INDUSTRY_UTILITIES_POWERPRODUCERS
```

---

### INDUSTRY_UTILITIES_RENEWABLE
```mql5
INDUSTRY_UTILITIES_RENEWABLE
```

---

### INDUSTRY_UTILITIES_REGULATED_ELECTRIC
```mql5
INDUSTRY_UTILITIES_REGULATED_ELECTRIC
```

---

### INDUSTRY_UTILITIES_REGULATED_GAS
```mql5
INDUSTRY_UTILITIES_REGULATED_GAS
```

---

### INDUSTRY_UTILITIES_REGULATED_WATER
```mql5
INDUSTRY_UTILITIES_REGULATED_WATER
```

---

### INDUSTRY_UTILITIES_FIRST
```mql5
INDUSTRY_UTILITIES_FIRST
```

---

### INDUSTRY_UTILITIES_LAST
```mql5
INDUSTRY_UTILITIES_LAST
```

---

### ENUM_ACCOUNT_INFO_INTEGER
```mql5
ENUM_ACCOUNT_INFO_INTEGER
```

---

### ACCOUNT_LOGIN
```mql5
ACCOUNT_LOGIN
```

---

### ACCOUNT_TRADE_MODE
```mql5
ACCOUNT_TRADE_MODE
```

---

### ACCOUNT_LEVERAGE
```mql5
ACCOUNT_LEVERAGE
```

---

### ACCOUNT_LIMIT_ORDERS
```mql5
ACCOUNT_LIMIT_ORDERS
```

---

### ACCOUNT_MARGIN_SO_MODE
```mql5
ACCOUNT_MARGIN_SO_MODE
```

---

### ACCOUNT_TRADE_ALLOWED
```mql5
ACCOUNT_TRADE_ALLOWED
```

---

### ACCOUNT_TRADE_EXPERT
```mql5
ACCOUNT_TRADE_EXPERT
```

---

### ACCOUNT_MARGIN_MODE
```mql5
ACCOUNT_MARGIN_MODE
```

---

### ACCOUNT_CURRENCY_DIGITS
```mql5
ACCOUNT_CURRENCY_DIGITS
```

---

### ACCOUNT_FIFO_CLOSE
```mql5
ACCOUNT_FIFO_CLOSE
```

---

### ACCOUNT_HEDGE_ALLOWED
```mql5
ACCOUNT_HEDGE_ALLOWED
```

---

### ENUM_ACCOUNT_INFO_DOUBLE
```mql5
ENUM_ACCOUNT_INFO_DOUBLE
```

---

### ACCOUNT_BALANCE
```mql5
ACCOUNT_BALANCE
```

---

### ACCOUNT_CREDIT
```mql5
ACCOUNT_CREDIT
```

---

### ACCOUNT_PROFIT
```mql5
ACCOUNT_PROFIT
```

---

### ACCOUNT_EQUITY
```mql5
ACCOUNT_EQUITY
```

---

### ACCOUNT_MARGIN
```mql5
ACCOUNT_MARGIN
```

---

### ACCOUNT_MARGIN_FREE
```mql5
ACCOUNT_MARGIN_FREE
```

---

### ACCOUNT_MARGIN_LEVEL
```mql5
ACCOUNT_MARGIN_LEVEL
```

---

### ACCOUNT_MARGIN_SO_CALL
```mql5
ACCOUNT_MARGIN_SO_CALL
```

---

### ACCOUNT_MARGIN_SO_SO
```mql5
ACCOUNT_MARGIN_SO_SO
```

---

### ACCOUNT_MARGIN_INITIAL
```mql5
ACCOUNT_MARGIN_INITIAL
```

---

### ACCOUNT_MARGIN_MAINTENANCE
```mql5
ACCOUNT_MARGIN_MAINTENANCE
```

---

### ACCOUNT_ASSETS
```mql5
ACCOUNT_ASSETS
```

---

### ACCOUNT_LIABILITIES
```mql5
ACCOUNT_LIABILITIES
```

---

### ACCOUNT_COMMISSION_BLOCKED
```mql5
ACCOUNT_COMMISSION_BLOCKED
```

---

### ENUM_ACCOUNT_INFO_STRING
```mql5
ENUM_ACCOUNT_INFO_STRING
```

---

### ACCOUNT_NAME
```mql5
ACCOUNT_NAME
```

---

### ACCOUNT_SERVER
```mql5
ACCOUNT_SERVER
```

---

### ACCOUNT_CURRENCY
```mql5
ACCOUNT_CURRENCY
```

---

### ACCOUNT_COMPANY
```mql5
ACCOUNT_COMPANY
```

---

### ENUM_ACCOUNT_TRADE_MODE
```mql5
ENUM_ACCOUNT_TRADE_MODE
```

---

### ACCOUNT_TRADE_MODE_DEMO
```mql5
ACCOUNT_TRADE_MODE_DEMO
```

---

### ACCOUNT_TRADE_MODE_CONTEST
```mql5
ACCOUNT_TRADE_MODE_CONTEST
```

---

### ACCOUNT_TRADE_MODE_REAL
```mql5
ACCOUNT_TRADE_MODE_REAL
```

---

### ENUM_ACCOUNT_STOPOUT_MODE
```mql5
ENUM_ACCOUNT_STOPOUT_MODE
```

---

### ACCOUNT_STOPOUT_MODE_PERCENT
```mql5
ACCOUNT_STOPOUT_MODE_PERCENT
```

---

### ACCOUNT_STOPOUT_MODE_MONEY
```mql5
ACCOUNT_STOPOUT_MODE_MONEY
```

---

### ENUM_ACCOUNT_MARGIN_MODE
```mql5
ENUM_ACCOUNT_MARGIN_MODE
```

---

### ACCOUNT_MARGIN_MODE_RETAIL_NETTING
```mql5
ACCOUNT_MARGIN_MODE_RETAIL_NETTING
```

---

### ACCOUNT_MARGIN_MODE_EXCHANGE
```mql5
ACCOUNT_MARGIN_MODE_EXCHANGE
```

---

### ACCOUNT_MARGIN_MODE_RETAIL_HEDGING
```mql5
ACCOUNT_MARGIN_MODE_RETAIL_HEDGING
```

---

### ENUM_STATISTICS
```mql5
ENUM_STATISTICS
```

---

### STAT_INITIAL_DEPOSIT
```mql5
STAT_INITIAL_DEPOSIT
```

---

### STAT_WITHDRAWAL
```mql5
STAT_WITHDRAWAL
```

---

### STAT_PROFIT
```mql5
STAT_PROFIT
```

---

### STAT_GROSS_PROFIT
```mql5
STAT_GROSS_PROFIT
```

---

### STAT_GROSS_LOSS
```mql5
STAT_GROSS_LOSS
```

---

### STAT_MAX_PROFITTRADE
```mql5
STAT_MAX_PROFITTRADE
```

---

### STAT_MAX_LOSSTRADE
```mql5
STAT_MAX_LOSSTRADE
```

---

### STAT_CONPROFITMAX
```mql5
STAT_CONPROFITMAX
```

---

### STAT_CONPROFITMAX_TRADES
```mql5
STAT_CONPROFITMAX_TRADES
```

---

### STAT_MAX_CONWINS
```mql5
STAT_MAX_CONWINS
```

---

### STAT_MAX_CONPROFIT_TRADES
```mql5
STAT_MAX_CONPROFIT_TRADES
```

---

### STAT_CONLOSSMAX
```mql5
STAT_CONLOSSMAX
```

---

### STAT_CONLOSSMAX_TRADES
```mql5
STAT_CONLOSSMAX_TRADES
```

---

### STAT_MAX_CONLOSSES
```mql5
STAT_MAX_CONLOSSES
```

---

### STAT_MAX_CONLOSS_TRADES
```mql5
STAT_MAX_CONLOSS_TRADES
```

---

### STAT_BALANCEMIN
```mql5
STAT_BALANCEMIN
```

---

### STAT_BALANCE_DD
```mql5
STAT_BALANCE_DD
```

---

### STAT_BALANCEDD_PERCENT
```mql5
STAT_BALANCEDD_PERCENT
```

---

### STAT_BALANCE_DDREL_PERCENT
```mql5
STAT_BALANCE_DDREL_PERCENT
```

---

### STAT_BALANCE_DD_RELATIVE
```mql5
STAT_BALANCE_DD_RELATIVE
```

---

### STAT_EQUITYMIN
```mql5
STAT_EQUITYMIN
```

---

### STAT_EQUITY_DD
```mql5
STAT_EQUITY_DD
```

---

### STAT_EQUITYDD_PERCENT
```mql5
STAT_EQUITYDD_PERCENT
```

---

### STAT_EQUITY_DDREL_PERCENT
```mql5
STAT_EQUITY_DDREL_PERCENT
```

---

### STAT_EQUITY_DD_RELATIVE
```mql5
STAT_EQUITY_DD_RELATIVE
```

---

### STAT_EXPECTED_PAYOFF
```mql5
STAT_EXPECTED_PAYOFF
```

---

### STAT_PROFIT_FACTOR
```mql5
STAT_PROFIT_FACTOR
```

---

### STAT_RECOVERY_FACTOR
```mql5
STAT_RECOVERY_FACTOR
```

---

### STAT_SHARPE_RATIO
```mql5
STAT_SHARPE_RATIO
```

---

### STAT_MIN_MARGINLEVEL
```mql5
STAT_MIN_MARGINLEVEL
```

---

### STAT_CUSTOM_ONTESTER
```mql5
STAT_CUSTOM_ONTESTER
```

---

### STAT_DEALS
```mql5
STAT_DEALS
```

---

### STAT_TRADES
```mql5
STAT_TRADES
```

---

### STAT_PROFIT_TRADES
```mql5
STAT_PROFIT_TRADES
```

---

### STAT_LOSS_TRADES
```mql5
STAT_LOSS_TRADES
```

---

### STAT_SHORT_TRADES
```mql5
STAT_SHORT_TRADES
```

---

### STAT_LONG_TRADES
```mql5
STAT_LONG_TRADES
```

---

### STAT_PROFIT_SHORTTRADES
```mql5
STAT_PROFIT_SHORTTRADES
```

---

### STAT_PROFIT_LONGTRADES
```mql5
STAT_PROFIT_LONGTRADES
```

---

### STAT_PROFITTRADES_AVGCON
```mql5
STAT_PROFITTRADES_AVGCON
```

---

### STAT_LOSSTRADES_AVGCON
```mql5
STAT_LOSSTRADES_AVGCON
```

---

### TRADE_RETCODE_REQUOTE
```mql5
TRADE_RETCODE_REQUOTE
```

---

### TRADE_RETCODE_REJECT
```mql5
TRADE_RETCODE_REJECT
```

---

### TRADE_RETCODE_CANCEL
```mql5
TRADE_RETCODE_CANCEL
```

---

### TRADE_RETCODE_PLACED
```mql5
TRADE_RETCODE_PLACED
```

---

### TRADE_RETCODE_DONE
```mql5
TRADE_RETCODE_DONE
```

---

### TRADE_RETCODE_DONE_PARTIAL
```mql5
TRADE_RETCODE_DONE_PARTIAL
```

---

### TRADE_RETCODE_ERROR
```mql5
TRADE_RETCODE_ERROR
```

---

### TRADE_RETCODE_TIMEOUT
```mql5
TRADE_RETCODE_TIMEOUT
```

---

### TRADE_RETCODE_INVALID
```mql5
TRADE_RETCODE_INVALID
```

---

### TRADE_RETCODE_INVALID_VOLUME
```mql5
TRADE_RETCODE_INVALID_VOLUME
```

---

### TRADE_RETCODE_INVALID_PRICE
```mql5
TRADE_RETCODE_INVALID_PRICE
```

---

### TRADE_RETCODE_INVALID_STOPS
```mql5
TRADE_RETCODE_INVALID_STOPS
```

---

### TRADE_RETCODE_TRADE_DISABLED
```mql5
TRADE_RETCODE_TRADE_DISABLED
```

---

### TRADE_RETCODE_MARKET_CLOSED
```mql5
TRADE_RETCODE_MARKET_CLOSED
```

---

### TRADE_RETCODE_NO_MONEY
```mql5
TRADE_RETCODE_NO_MONEY
```

---

### TRADE_RETCODE_PRICE_CHANGED
```mql5
TRADE_RETCODE_PRICE_CHANGED
```

---

### TRADE_RETCODE_PRICE_OFF
```mql5
TRADE_RETCODE_PRICE_OFF
```

---

### TRADE_RETCODE_INVALID_EXPIRATION
```mql5
TRADE_RETCODE_INVALID_EXPIRATION
```

---

### TRADE_RETCODE_ORDER_CHANGED
```mql5
TRADE_RETCODE_ORDER_CHANGED
```

---

### TRADE_RETCODE_TOO_MANY_REQUESTS
```mql5
TRADE_RETCODE_TOO_MANY_REQUESTS
```

---

### TRADE_RETCODE_NO_CHANGES
```mql5
TRADE_RETCODE_NO_CHANGES
```

---

### TRADE_RETCODE_SERVER_DISABLES_AT
```mql5
TRADE_RETCODE_SERVER_DISABLES_AT
```

---

### TRADE_RETCODE_CLIENT_DISABLES_AT
```mql5
TRADE_RETCODE_CLIENT_DISABLES_AT
```

---

### TRADE_RETCODE_LOCKED
```mql5
TRADE_RETCODE_LOCKED
```

---

### TRADE_RETCODE_FROZEN
```mql5
TRADE_RETCODE_FROZEN
```

---

### TRADE_RETCODE_INVALID_FILL
```mql5
TRADE_RETCODE_INVALID_FILL
```

---

### TRADE_RETCODE_CONNECTION
```mql5
TRADE_RETCODE_CONNECTION
```

---

### TRADE_RETCODE_ONLY_REAL
```mql5
TRADE_RETCODE_ONLY_REAL
```

---

### TRADE_RETCODE_LIMIT_ORDERS
```mql5
TRADE_RETCODE_LIMIT_ORDERS
```

---

### TRADE_RETCODE_LIMIT_VOLUME
```mql5
TRADE_RETCODE_LIMIT_VOLUME
```

---

### TRADE_RETCODE_INVALID_ORDER
```mql5
TRADE_RETCODE_INVALID_ORDER
```

---

### TRADE_RETCODE_POSITION_CLOSED
```mql5
TRADE_RETCODE_POSITION_CLOSED
```

---

### TRADE_RETCODE_INVALID_CLOSE_VOLUME
```mql5
TRADE_RETCODE_INVALID_CLOSE_VOLUME
```

---

### TRADE_RETCODE_CLOSE_ORDER_EXIST
```mql5
TRADE_RETCODE_CLOSE_ORDER_EXIST
```

---

### TRADE_RETCODE_LIMIT_POSITIONS
```mql5
TRADE_RETCODE_LIMIT_POSITIONS
```

---

### TRADE_RETCODE_REJECT_CANCEL
```mql5
TRADE_RETCODE_REJECT_CANCEL
```

---

### TRADE_RETCODE_LONG_ONLY
```mql5
TRADE_RETCODE_LONG_ONLY
```

---

### TRADE_RETCODE_SHORT_ONLY
```mql5
TRADE_RETCODE_SHORT_ONLY
```

---

### TRADE_RETCODE_CLOSE_ONLY
```mql5
TRADE_RETCODE_CLOSE_ONLY
```

---

### TRADE_RETCODE_FIFO_CLOSE
```mql5
TRADE_RETCODE_FIFO_CLOSE
```

---

### TRADE_RETCODE_HEDGE_PROHIBITED
```mql5
TRADE_RETCODE_HEDGE_PROHIBITED
```

---

### ERR_SUCCESS
```mql5
ERR_SUCCESS
```

---

### ERR_INTERNAL_ERROR
```mql5
ERR_INTERNAL_ERROR
```

---

### ERR_WRONG_INTERNAL_PARAMETER
```mql5
ERR_WRONG_INTERNAL_PARAMETER
```

---

### ERR_INVALID_PARAMETER
```mql5
ERR_INVALID_PARAMETER
```

---

### ERR_NOT_ENOUGH_MEMORY
```mql5
ERR_NOT_ENOUGH_MEMORY
```

---

### ERR_STRUCT_WITHOBJECTS_ORCLASS
```mql5
ERR_STRUCT_WITHOBJECTS_ORCLASS
```

---

### ERR_INVALID_ARRAY
```mql5
ERR_INVALID_ARRAY
```

---

### ERR_ARRAY_RESIZE_ERROR
```mql5
ERR_ARRAY_RESIZE_ERROR
```

---

### ERR_STRING_RESIZE_ERROR
```mql5
ERR_STRING_RESIZE_ERROR
```

---

### ERR_NOTINITIALIZED_STRING
```mql5
ERR_NOTINITIALIZED_STRING
```

---

### ERR_INVALID_DATETIME
```mql5
ERR_INVALID_DATETIME
```

---

### ERR_ARRAY_BAD_SIZE
```mql5
ERR_ARRAY_BAD_SIZE
```

---

### ERR_INVALID_POINTER
```mql5
ERR_INVALID_POINTER
```

---

### ERR_INVALID_POINTER_TYPE
```mql5
ERR_INVALID_POINTER_TYPE
```

---

### ERR_FUNCTION_NOT_ALLOWED
```mql5
ERR_FUNCTION_NOT_ALLOWED
```

---

### ERR_RESOURCE_NAME_DUPLICATED
```mql5
ERR_RESOURCE_NAME_DUPLICATED
```

---

### ERR_RESOURCE_NOT_FOUND
```mql5
ERR_RESOURCE_NOT_FOUND
```

---

### ERR_RESOURCE_UNSUPPOTED_TYPE
```mql5
ERR_RESOURCE_UNSUPPOTED_TYPE
```

---

### ERR_RESOURCE_NAME_IS_TOO_LONG
```mql5
ERR_RESOURCE_NAME_IS_TOO_LONG
```

---

### ERR_MATH_OVERFLOW
```mql5
ERR_MATH_OVERFLOW
```

---

### ERR_SLEEP_ERROR
```mql5
ERR_SLEEP_ERROR
```

---

### ERR_PROGRAM_STOPPED
```mql5
ERR_PROGRAM_STOPPED
```

---

### ERR_CHART_WRONG_ID
```mql5
ERR_CHART_WRONG_ID
```

---

### ERR_CHART_NO_REPLY
```mql5
ERR_CHART_NO_REPLY
```

---

### ERR_CHART_NOT_FOUND
```mql5
ERR_CHART_NOT_FOUND
```

---

### ERR_CHART_NO_EXPERT
```mql5
ERR_CHART_NO_EXPERT
```

---

### ERR_CHART_CANNOT_OPEN
```mql5
ERR_CHART_CANNOT_OPEN
```

---

### ERR_CHART_CANNOT_CHANGE
```mql5
ERR_CHART_CANNOT_CHANGE
```

---

### ERR_CHART_WRONG_PARAMETER
```mql5
ERR_CHART_WRONG_PARAMETER
```

---

### ERR_CHART_CANNOT_CREATE_TIMER
```mql5
ERR_CHART_CANNOT_CREATE_TIMER
```

---

### ERR_CHART_WRONG_PROPERTY
```mql5
ERR_CHART_WRONG_PROPERTY
```

---

### ERR_CHART_SCREENSHOT_FAILED
```mql5
ERR_CHART_SCREENSHOT_FAILED
```

---

### ERR_CHART_NAVIGATE_FAILED
```mql5
ERR_CHART_NAVIGATE_FAILED
```

---

### ERR_CHART_TEMPLATE_FAILED
```mql5
ERR_CHART_TEMPLATE_FAILED
```

---

### ERR_CHART_WINDOW_NOT_FOUND
```mql5
ERR_CHART_WINDOW_NOT_FOUND
```

---

### ERR_CHART_INDICATOR_CANNOT_ADD
```mql5
ERR_CHART_INDICATOR_CANNOT_ADD
```

---

### ERR_CHART_INDICATOR_CANNOT_DEL
```mql5
ERR_CHART_INDICATOR_CANNOT_DEL
```

---

### ERR_CHART_INDICATOR_NOT_FOUND
```mql5
ERR_CHART_INDICATOR_NOT_FOUND
```

---

### ERR_OBJECT_ERROR
```mql5
ERR_OBJECT_ERROR
```

---

### ERR_OBJECT_NOT_FOUND
```mql5
ERR_OBJECT_NOT_FOUND
```

---

### ERR_OBJECT_WRONG_PROPERTY
```mql5
ERR_OBJECT_WRONG_PROPERTY
```

---

### ERR_OBJECT_GETDATE_FAILED
```mql5
ERR_OBJECT_GETDATE_FAILED
```

---

### ERR_OBJECT_GETVALUE_FAILED
```mql5
ERR_OBJECT_GETVALUE_FAILED
```

---

### ERR_MARKET_UNKNOWN_SYMBOL
```mql5
ERR_MARKET_UNKNOWN_SYMBOL
```

---

### ERR_MARKET_NOT_SELECTED
```mql5
ERR_MARKET_NOT_SELECTED
```

---

### ERR_MARKET_WRONG_PROPERTY
```mql5
ERR_MARKET_WRONG_PROPERTY
```

---

### ERR_MARKET_LASTTIME_UNKNOWN
```mql5
ERR_MARKET_LASTTIME_UNKNOWN
```

---

### ERR_MARKET_SELECT_ERROR
```mql5
ERR_MARKET_SELECT_ERROR
```

---

### ERR_HISTORY_NOT_FOUND
```mql5
ERR_HISTORY_NOT_FOUND
```

---

### ERR_HISTORY_WRONG_PROPERTY
```mql5
ERR_HISTORY_WRONG_PROPERTY
```

---

### ERR_HISTORY_TIMEOUT
```mql5
ERR_HISTORY_TIMEOUT
```

---

### ERR_HISTORY_BARS_LIMIT
```mql5
ERR_HISTORY_BARS_LIMIT
```

---

### ERR_HISTORY_LOAD_ERRORS
```mql5
ERR_HISTORY_LOAD_ERRORS
```

---

### ERR_HISTORY_SMALL_BUFFER
```mql5
ERR_HISTORY_SMALL_BUFFER
```

---

### ERR_GLOBALVARIABLE_NOT_FOUND
```mql5
ERR_GLOBALVARIABLE_NOT_FOUND
```

---

### ERR_GLOBALVARIABLE_EXISTS
```mql5
ERR_GLOBALVARIABLE_EXISTS
```

---

### ERR_GLOBALVARIABLE_NOT_MODIFIED
```mql5
ERR_GLOBALVARIABLE_NOT_MODIFIED
```

---

### ERR_GLOBALVARIABLE_CANNOTREAD
```mql5
ERR_GLOBALVARIABLE_CANNOTREAD
```

---

### ERR_GLOBALVARIABLE_CANNOTWRITE
```mql5
ERR_GLOBALVARIABLE_CANNOTWRITE
```

---

### ERR_MAIL_SEND_FAILED
```mql5
ERR_MAIL_SEND_FAILED
```

---

### ERR_PLAY_SOUND_FAILED
```mql5
ERR_PLAY_SOUND_FAILED
```

---

### ERR_MQL5_WRONG_PROPERTY
```mql5
ERR_MQL5_WRONG_PROPERTY
```

---

### ERR_TERMINAL_WRONG_PROPERTY
```mql5
ERR_TERMINAL_WRONG_PROPERTY
```

---

### ERR_FTP_SEND_FAILED
```mql5
ERR_FTP_SEND_FAILED
```

---

### ERR_NOTIFICATION_SEND_FAILED
```mql5
ERR_NOTIFICATION_SEND_FAILED
```

---

### ERR_NOTIFICATION_WRONG_PARAMETER
```mql5
ERR_NOTIFICATION_WRONG_PARAMETER
```

---

### ERR_NOTIFICATION_WRONG_SETTINGS
```mql5
ERR_NOTIFICATION_WRONG_SETTINGS
```

---

### ERR_NOTIFICATION_TOO_FREQUENT
```mql5
ERR_NOTIFICATION_TOO_FREQUENT
```

---

### ERR_FTP_NOSERVER
```mql5
ERR_FTP_NOSERVER
```

---

### ERR_FTP_NOLOGIN
```mql5
ERR_FTP_NOLOGIN
```

---

### ERR_FTP_FILE_ERROR
```mql5
ERR_FTP_FILE_ERROR
```

---

### ERR_FTP_CONNECT_FAILED
```mql5
ERR_FTP_CONNECT_FAILED
```

---

### ERR_FTP_CHANGEDIR
```mql5
ERR_FTP_CHANGEDIR
```

---

### ERR_FTP_CLOSED
```mql5
ERR_FTP_CLOSED
```

---

### ERR_BUFFERS_NO_MEMORY
```mql5
ERR_BUFFERS_NO_MEMORY
```

---

### ERR_BUFFERS_WRONG_INDEX
```mql5
ERR_BUFFERS_WRONG_INDEX
```

---

### ERR_CUSTOM_WRONG_PROPERTY
```mql5
ERR_CUSTOM_WRONG_PROPERTY
```

---

### ERR_ACCOUNT_WRONG_PROPERTY
```mql5
ERR_ACCOUNT_WRONG_PROPERTY
```

---

### ERR_TRADE_WRONG_PROPERTY
```mql5
ERR_TRADE_WRONG_PROPERTY
```

---

### ERR_TRADE_DISABLED
```mql5
ERR_TRADE_DISABLED
```

---

### ERR_TRADE_POSITION_NOT_FOUND
```mql5
ERR_TRADE_POSITION_NOT_FOUND
```

---

### ERR_TRADE_ORDER_NOT_FOUND
```mql5
ERR_TRADE_ORDER_NOT_FOUND
```

---

### ERR_TRADE_DEAL_NOT_FOUND
```mql5
ERR_TRADE_DEAL_NOT_FOUND
```

---

### ERR_TRADE_SEND_FAILED
```mql5
ERR_TRADE_SEND_FAILED
```

---

### ERR_TRADE_CALC_FAILED
```mql5
ERR_TRADE_CALC_FAILED
```

---

### ERR_INDICATOR_UNKNOWN_SYMBOL
```mql5
ERR_INDICATOR_UNKNOWN_SYMBOL
```

---

### ERR_INDICATOR_CANNOT_CREATE
```mql5
ERR_INDICATOR_CANNOT_CREATE
```

---

### ERR_INDICATOR_NO_MEMORY
```mql5
ERR_INDICATOR_NO_MEMORY
```

---

### ERR_INDICATOR_CANNOT_APPLY
```mql5
ERR_INDICATOR_CANNOT_APPLY
```

---

### ERR_INDICATOR_CANNOT_ADD
```mql5
ERR_INDICATOR_CANNOT_ADD
```

---

### ERR_INDICATOR_DATA_NOT_FOUND
```mql5
ERR_INDICATOR_DATA_NOT_FOUND
```

---

### ERR_INDICATOR_WRONG_HANDLE
```mql5
ERR_INDICATOR_WRONG_HANDLE
```

---

### ERR_INDICATOR_WRONG_PARAMETERS
```mql5
ERR_INDICATOR_WRONG_PARAMETERS
```

---

### ERR_INDICATOR_PARAMETERS_MISSING
```mql5
ERR_INDICATOR_PARAMETERS_MISSING
```

---

### ERR_INDICATOR_CUSTOM_NAME
```mql5
ERR_INDICATOR_CUSTOM_NAME
```

---

### ERR_INDICATOR_PARAMETER_TYPE
```mql5
ERR_INDICATOR_PARAMETER_TYPE
```

---

### ERR_INDICATOR_WRONG_INDEX
```mql5
ERR_INDICATOR_WRONG_INDEX
```

---

### ERR_BOOKS_CANNOT_ADD
```mql5
ERR_BOOKS_CANNOT_ADD
```

---

### ERR_BOOKS_CANNOT_DELETE
```mql5
ERR_BOOKS_CANNOT_DELETE
```

---

### ERR_BOOKS_CANNOT_GET
```mql5
ERR_BOOKS_CANNOT_GET
```

---

### ERR_BOOKS_CANNOT_SUBSCRIBE
```mql5
ERR_BOOKS_CANNOT_SUBSCRIBE
```

---

### ERR_TOO_MANY_FILES
```mql5
ERR_TOO_MANY_FILES
```

---

### ERR_WRONG_FILENAME
```mql5
ERR_WRONG_FILENAME
```

---

### ERR_TOO_LONG_FILENAME
```mql5
ERR_TOO_LONG_FILENAME
```

---

### ERR_CANNOT_OPEN_FILE
```mql5
ERR_CANNOT_OPEN_FILE
```

---

### ERR_FILE_CACHEBUFFER_ERROR
```mql5
ERR_FILE_CACHEBUFFER_ERROR
```

---

### ERR_CANNOT_DELETE_FILE
```mql5
ERR_CANNOT_DELETE_FILE
```

---

### ERR_INVALID_FILEHANDLE
```mql5
ERR_INVALID_FILEHANDLE
```

---

### ERR_WRONG_FILEHANDLE
```mql5
ERR_WRONG_FILEHANDLE
```

---

### ERR_FILE_NOTTOWRITE
```mql5
ERR_FILE_NOTTOWRITE
```

---

### ERR_FILE_NOTTOREAD
```mql5
ERR_FILE_NOTTOREAD
```

---

### ERR_FILE_NOTBIN
```mql5
ERR_FILE_NOTBIN
```

---

### ERR_FILE_NOTTXT
```mql5
ERR_FILE_NOTTXT
```

---

### ERR_FILE_NOTTXTORCSV
```mql5
ERR_FILE_NOTTXTORCSV
```

---

### ERR_FILE_NOTCSV
```mql5
ERR_FILE_NOTCSV
```

---

### ERR_FILE_READERROR
```mql5
ERR_FILE_READERROR
```

---

### ERR_FILE_BINSTRINGSIZE
```mql5
ERR_FILE_BINSTRINGSIZE
```

---

### ERR_INCOMPATIBLE_FILE
```mql5
ERR_INCOMPATIBLE_FILE
```

---

### ERR_FILE_IS_DIRECTORY
```mql5
ERR_FILE_IS_DIRECTORY
```

---

### ERR_FILE_NOT_EXIST
```mql5
ERR_FILE_NOT_EXIST
```

---

### ERR_FILE_CANNOT_REWRITE
```mql5
ERR_FILE_CANNOT_REWRITE
```

---

### ERR_WRONG_DIRECTORYNAME
```mql5
ERR_WRONG_DIRECTORYNAME
```

---

### ERR_DIRECTORY_NOT_EXIST
```mql5
ERR_DIRECTORY_NOT_EXIST
```

---

### ERR_FILE_ISNOT_DIRECTORY
```mql5
ERR_FILE_ISNOT_DIRECTORY
```

---

### ERR_CANNOT_DELETE_DIRECTORY
```mql5
ERR_CANNOT_DELETE_DIRECTORY
```

---

### ERR_CANNOT_CLEAN_DIRECTORY
```mql5
ERR_CANNOT_CLEAN_DIRECTORY
```

---

### ERR_FILE_WRITEERROR
```mql5
ERR_FILE_WRITEERROR
```

---

### ERR_FILE_ENDOFFILE
```mql5
ERR_FILE_ENDOFFILE
```

---

### ERR_NO_STRING_DATE
```mql5
ERR_NO_STRING_DATE
```

---

### ERR_WRONG_STRING_DATE
```mql5
ERR_WRONG_STRING_DATE
```

---

### ERR_WRONG_STRING_TIME
```mql5
ERR_WRONG_STRING_TIME
```

---

### ERR_STRING_TIME_ERROR
```mql5
ERR_STRING_TIME_ERROR
```

---

### ERR_STRING_OUT_OF_MEMORY
```mql5
ERR_STRING_OUT_OF_MEMORY
```

---

### ERR_STRING_SMALL_LEN
```mql5
ERR_STRING_SMALL_LEN
```

---

### ERR_STRING_TOO_BIGNUMBER
```mql5
ERR_STRING_TOO_BIGNUMBER
```

---

### ERR_WRONG_FORMATSTRING
```mql5
ERR_WRONG_FORMATSTRING
```

---

### ERR_TOO_MANY_FORMATTERS
```mql5
ERR_TOO_MANY_FORMATTERS
```

---

### ERR_TOO_MANY_PARAMETERS
```mql5
ERR_TOO_MANY_PARAMETERS
```

---

### ERR_WRONG_STRING_PARAMETER
```mql5
ERR_WRONG_STRING_PARAMETER
```

---

### ERR_STRINGPOS_OUTOFRANGE
```mql5
ERR_STRINGPOS_OUTOFRANGE
```

---

### ERR_STRING_ZEROADDED
```mql5
ERR_STRING_ZEROADDED
```

---

### ERR_STRING_UNKNOWNTYPE
```mql5
ERR_STRING_UNKNOWNTYPE
```

---

### ERR_WRONG_STRING_OBJECT
```mql5
ERR_WRONG_STRING_OBJECT
```

---

### ERR_INCOMPATIBLE_ARRAYS
```mql5
ERR_INCOMPATIBLE_ARRAYS
```

---

### ERR_SMALL_ASSERIES_ARRAY
```mql5
ERR_SMALL_ASSERIES_ARRAY
```

---

### ERR_SMALL_ARRAY
```mql5
ERR_SMALL_ARRAY
```

---

### ERR_ZEROSIZE_ARRAY
```mql5
ERR_ZEROSIZE_ARRAY
```

---

### ERR_NUMBER_ARRAYS_ONLY
```mql5
ERR_NUMBER_ARRAYS_ONLY
```

---

### ERR_ONEDIM_ARRAYS_ONLY
```mql5
ERR_ONEDIM_ARRAYS_ONLY
```

---

### ERR_SERIES_ARRAY
```mql5
ERR_SERIES_ARRAY
```

---

### ERR_DOUBLE_ARRAY_ONLY
```mql5
ERR_DOUBLE_ARRAY_ONLY
```

---

### ERR_FLOAT_ARRAY_ONLY
```mql5
ERR_FLOAT_ARRAY_ONLY
```

---

### ERR_LONG_ARRAY_ONLY
```mql5
ERR_LONG_ARRAY_ONLY
```

---

### ERR_INT_ARRAY_ONLY
```mql5
ERR_INT_ARRAY_ONLY
```

---

### ERR_SHORT_ARRAY_ONLY
```mql5
ERR_SHORT_ARRAY_ONLY
```

---

### ERR_CHAR_ARRAY_ONLY
```mql5
ERR_CHAR_ARRAY_ONLY
```

---

### ERR_STRING_ARRAY_ONLY
```mql5
ERR_STRING_ARRAY_ONLY
```

---

### ERR_OPENCL_NOT_SUPPORTED
```mql5
ERR_OPENCL_NOT_SUPPORTED
```

---

### ERR_OPENCL_INTERNAL
```mql5
ERR_OPENCL_INTERNAL
```

---

### ERR_OPENCL_INVALID_HANDLE
```mql5
ERR_OPENCL_INVALID_HANDLE
```

---

### ERR_OPENCL_CONTEXT_CREATE
```mql5
ERR_OPENCL_CONTEXT_CREATE
```

---

### ERR_OPENCL_QUEUE_CREATE
```mql5
ERR_OPENCL_QUEUE_CREATE
```

---

### ERR_OPENCL_PROGRAM_CREATE
```mql5
ERR_OPENCL_PROGRAM_CREATE
```

---

### ERR_OPENCL_TOO_LONG_KERNEL_NAME
```mql5
ERR_OPENCL_TOO_LONG_KERNEL_NAME
```

---

### ERR_OPENCL_KERNEL_CREATE
```mql5
ERR_OPENCL_KERNEL_CREATE
```

---

### ERR_OPENCL_SET_KERNEL_PARAMETER
```mql5
ERR_OPENCL_SET_KERNEL_PARAMETER
```

---

### ERR_OPENCL_EXECUTE
```mql5
ERR_OPENCL_EXECUTE
```

---

### ERR_OPENCL_WRONG_BUFFER_SIZE
```mql5
ERR_OPENCL_WRONG_BUFFER_SIZE
```

---

### ERR_OPENCL_WRONG_BUFFER_OFFSET
```mql5
ERR_OPENCL_WRONG_BUFFER_OFFSET
```

---

### ERR_OPENCL_BUFFER_CREATE
```mql5
ERR_OPENCL_BUFFER_CREATE
```

---

### ERR_OPENCL_TOO_MANY_OBJECTS
```mql5
ERR_OPENCL_TOO_MANY_OBJECTS
```

---

### ERR_OPENCL_SELECTDEVICE
```mql5
ERR_OPENCL_SELECTDEVICE
```

---

### ERR_DATABASE_INTERNAL
```mql5
ERR_DATABASE_INTERNAL
```

---

### ERR_DATABASE_INVALID_HANDLE
```mql5
ERR_DATABASE_INVALID_HANDLE
```

---

### ERR_DATABASE_TOO_MANY_OBJECTS
```mql5
ERR_DATABASE_TOO_MANY_OBJECTS
```

---

### ERR_DATABASE_CONNECT
```mql5
ERR_DATABASE_CONNECT
```

---

### ERR_DATABASE_EXECUTE
```mql5
ERR_DATABASE_EXECUTE
```

---

### ERR_DATABASE_PREPARE
```mql5
ERR_DATABASE_PREPARE
```

---

### ERR_DATABASE_NO_MORE_DATA
```mql5
ERR_DATABASE_NO_MORE_DATA
```

---

### ERR_DATABASE_STEP
```mql5
ERR_DATABASE_STEP
```

---

### ERR_DATABASE_NOT_READY
```mql5
ERR_DATABASE_NOT_READY
```

---

### ERR_DATABASE_BIND_PARAMETERS
```mql5
ERR_DATABASE_BIND_PARAMETERS
```

---

### ERR_WEBREQUEST_INVALID_ADDRESS
```mql5
ERR_WEBREQUEST_INVALID_ADDRESS
```

---

### ERR_WEBREQUEST_CONNECT_FAILED
```mql5
ERR_WEBREQUEST_CONNECT_FAILED
```

---

### ERR_WEBREQUEST_TIMEOUT
```mql5
ERR_WEBREQUEST_TIMEOUT
```

---

### ERR_WEBREQUEST_REQUEST_FAILED
```mql5
ERR_WEBREQUEST_REQUEST_FAILED
```

---

### ERR_NETSOCKET_INVALIDHANDLE
```mql5
ERR_NETSOCKET_INVALIDHANDLE
```

---

### ERR_NETSOCKET_TOO_MANY_OPENED
```mql5
ERR_NETSOCKET_TOO_MANY_OPENED
```

---

### ERR_NETSOCKET_CANNOT_CONNECT
```mql5
ERR_NETSOCKET_CANNOT_CONNECT
```

---

### ERR_NETSOCKET_IO_ERROR
```mql5
ERR_NETSOCKET_IO_ERROR
```

---

### ERR_NETSOCKET_HANDSHAKE_FAILED
```mql5
ERR_NETSOCKET_HANDSHAKE_FAILED
```

---

### ERR_NETSOCKET_NO_CERTIFICATE
```mql5
ERR_NETSOCKET_NO_CERTIFICATE
```

---

### ERR_NOT_CUSTOM_SYMBOL
```mql5
ERR_NOT_CUSTOM_SYMBOL
```

---

### ERR_CUSTOM_SYMBOL_WRONG_NAME
```mql5
ERR_CUSTOM_SYMBOL_WRONG_NAME
```

---

### ERR_CUSTOM_SYMBOL_NAME_LONG
```mql5
ERR_CUSTOM_SYMBOL_NAME_LONG
```

---

### ERR_CUSTOM_SYMBOL_PATH_LONG
```mql5
ERR_CUSTOM_SYMBOL_PATH_LONG
```

---

### ERR_CUSTOM_SYMBOL_EXIST
```mql5
ERR_CUSTOM_SYMBOL_EXIST
```

---

### ERR_CUSTOM_SYMBOL_ERROR
```mql5
ERR_CUSTOM_SYMBOL_ERROR
```

---

### ERR_CUSTOM_SYMBOL_SELECTED
```mql5
ERR_CUSTOM_SYMBOL_SELECTED
```

---

### ERR_CUSTOM_SYMBOL_PROPERTY_WRONG
```mql5
ERR_CUSTOM_SYMBOL_PROPERTY_WRONG
```

---

### ERR_CUSTOM_SYMBOL_PARAMETER_ERROR
```mql5
ERR_CUSTOM_SYMBOL_PARAMETER_ERROR
```

---

### ERR_CUSTOM_SYMBOL_PARAMETER_LONG
```mql5
ERR_CUSTOM_SYMBOL_PARAMETER_LONG
```

---

### ERR_CUSTOM_TICKS_WRONG_ORDER
```mql5
ERR_CUSTOM_TICKS_WRONG_ORDER
```

---

### ERR_CALENDAR_MORE_DATA
```mql5
ERR_CALENDAR_MORE_DATA
```

---

### ERR_CALENDAR_TIMEOUT
```mql5
ERR_CALENDAR_TIMEOUT
```

---

### ERR_CALENDAR_NO_DATA
```mql5
ERR_CALENDAR_NO_DATA
```

---

### ERR_DATABASE_ERROR
```mql5
ERR_DATABASE_ERROR
```

---

### ERR_DATABASE_PERM
```mql5
ERR_DATABASE_PERM
```

---

### ERR_DATABASE_ABORT
```mql5
ERR_DATABASE_ABORT
```

---

### ERR_DATABASE_BUSY
```mql5
ERR_DATABASE_BUSY
```

---

### ERR_DATABASE_LOCKED
```mql5
ERR_DATABASE_LOCKED
```

---

### ERR_DATABASE_NOMEM
```mql5
ERR_DATABASE_NOMEM
```

---

### ERR_DATABASE_READONLY
```mql5
ERR_DATABASE_READONLY
```

---

### ERR_DATABASE_INTERRUPT
```mql5
ERR_DATABASE_INTERRUPT
```

---

### ERR_DATABASE_IOERR
```mql5
ERR_DATABASE_IOERR
```

---

### ERR_DATABASE_CORRUPT
```mql5
ERR_DATABASE_CORRUPT
```

---

### ERR_DATABASE_NOTFOUND
```mql5
ERR_DATABASE_NOTFOUND
```

---

### ERR_DATABASE_FULL
```mql5
ERR_DATABASE_FULL
```

---

### ERR_DATABASE_CANTOPEN
```mql5
ERR_DATABASE_CANTOPEN
```

---

### ERR_DATABASE_PROTOCOL
```mql5
ERR_DATABASE_PROTOCOL
```

---

### ERR_DATABASE_EMPTY
```mql5
ERR_DATABASE_EMPTY
```

---

### ERR_DATABASE_SCHEMA
```mql5
ERR_DATABASE_SCHEMA
```

---

### ERR_DATABASE_TOOBIG
```mql5
ERR_DATABASE_TOOBIG
```

---

### ERR_DATABASE_CONSTRAINT
```mql5
ERR_DATABASE_CONSTRAINT
```

---

### ERR_DATABASE_MISMATCH
```mql5
ERR_DATABASE_MISMATCH
```

---

### ERR_DATABASE_MISUSE
```mql5
ERR_DATABASE_MISUSE
```

---

### ERR_DATABASE_NOLFS
```mql5
ERR_DATABASE_NOLFS
```

---

### ERR_DATABASE_AUTH
```mql5
ERR_DATABASE_AUTH
```

---

### ERR_DATABASE_FORMAT
```mql5
ERR_DATABASE_FORMAT
```

---

### ERR_DATABASE_RANGE
```mql5
ERR_DATABASE_RANGE
```

---

### ERR_DATABASE_NOTADB
```mql5
ERR_DATABASE_NOTADB
```

---

### ERR_USER_ERROR_FIRST
```mql5
ERR_USER_ERROR_FIRST
```

---

### CArray
```mql5
CArray 
```

---

### CArrayChar
```mql5
CArrayChar 
```

---

### CArrayShort
```mql5
CArrayShort 
```

---

### CArrayInt
```mql5
CArrayInt 
```

---

### CArrayLong
```mql5
CArrayLong 
```

---

### CArrayFloat
```mql5
CArrayFloat 
```

---

### CArrayDouble
```mql5
CArrayDouble 
```

---

### CArrayString
```mql5
CArrayString 
```

---

### CArrayObj
```mql5
CArrayObj 
```

---

### CList
```mql5
CList 
```

---

### CTreeNode
```mql5
CTreeNode 
```

---

### CTree
```mql5
CTree 
```

---

### MqlTradeTransaction
```mql5
MqlTradeTransaction
```

---

### ENUM_CALENDAR_EVENT_FREQUENCY
```mql5
ENUM_CALENDAR_EVENT_FREQUENCY
```

---

### CALENDAR_FREQUENCY_NONE
```mql5
CALENDAR_FREQUENCY_NONE
```

---

### CALENDAR_FREQUENCY_WEEK
```mql5
CALENDAR_FREQUENCY_WEEK
```

---

### CALENDAR_FREQUENCY_MONTH
```mql5
CALENDAR_FREQUENCY_MONTH
```

---

### CALENDAR_FREQUENCY_QUARTER
```mql5
CALENDAR_FREQUENCY_QUARTER
```

---

### CALENDAR_FREQUENCY_YEAR
```mql5
CALENDAR_FREQUENCY_YEAR
```

---

### CALENDAR_FREQUENCY_DAY
```mql5
CALENDAR_FREQUENCY_DAY
```

---

### ENUM_CALENDAR_EVENT_TYPE
```mql5
ENUM_CALENDAR_EVENT_TYPE
```

---

### CALENDAR_TYPE_EVENT
```mql5
CALENDAR_TYPE_EVENT
```

---

### CALENDAR_TYPE_INDICATOR
```mql5
CALENDAR_TYPE_INDICATOR
```

---

### CALENDAR_TYPE_HOLIDAY
```mql5
CALENDAR_TYPE_HOLIDAY
```

---

### ENUM_CALENDAR_EVENT_SECTOR
```mql5
ENUM_CALENDAR_EVENT_SECTOR
```

---

### CALENDAR_SECTOR_NONE
```mql5
CALENDAR_SECTOR_NONE
```

---

### CALENDAR_SECTOR_MARKET
```mql5
CALENDAR_SECTOR_MARKET
```

---

### CALENDAR_SECTOR_GDP
```mql5
CALENDAR_SECTOR_GDP
```

---

### CALENDAR_SECTOR_JOBS
```mql5
CALENDAR_SECTOR_JOBS
```

---

### CALENDAR_SECTOR_PRICES
```mql5
CALENDAR_SECTOR_PRICES
```

---

### CALENDAR_SECTOR_MONEY
```mql5
CALENDAR_SECTOR_MONEY
```

---

### CALENDAR_SECTOR_TRADE
```mql5
CALENDAR_SECTOR_TRADE
```

---

### CALENDAR_SECTOR_GOVERNMENT
```mql5
CALENDAR_SECTOR_GOVERNMENT
```

---

### CALENDAR_SECTOR_BUSINESS
```mql5
CALENDAR_SECTOR_BUSINESS
```

---

### CALENDAR_SECTOR_CONSUMER
```mql5
CALENDAR_SECTOR_CONSUMER
```

---

### CALENDAR_SECTOR_HOUSING
```mql5
CALENDAR_SECTOR_HOUSING
```

---

### CALENDAR_SECTOR_TAXES
```mql5
CALENDAR_SECTOR_TAXES
```

---

### CALENDAR_SECTOR_HOLIDAYS
```mql5
CALENDAR_SECTOR_HOLIDAYS
```

---

### ENUM_CALENDAR_EVENT_IMPORTANCE
```mql5
ENUM_CALENDAR_EVENT_IMPORTANCE
```

---

### CALENDAR_IMPORTANCE_NONE
```mql5
CALENDAR_IMPORTANCE_NONE
```

---

### CALENDAR_IMPORTANCE_LOW
```mql5
CALENDAR_IMPORTANCE_LOW
```

---

### CALENDAR_IMPORTANCE_MODERATE
```mql5
CALENDAR_IMPORTANCE_MODERATE
```

---

### CALENDAR_IMPORTANCE_HIGH
```mql5
CALENDAR_IMPORTANCE_HIGH
```

---

### ENUM_CALENDAR_EVENT_UNIT
```mql5
ENUM_CALENDAR_EVENT_UNIT
```

---

### CALENDAR_UNIT_NONE
```mql5
CALENDAR_UNIT_NONE
```

---

### CALENDAR_UNIT_PERCENT
```mql5
CALENDAR_UNIT_PERCENT
```

---

### CALENDAR_UNIT_CURRENCY
```mql5
CALENDAR_UNIT_CURRENCY
```

---

### CALENDAR_UNIT_HOUR
```mql5
CALENDAR_UNIT_HOUR
```

---

### CALENDAR_UNIT_JOB
```mql5
CALENDAR_UNIT_JOB
```

---

### CALENDAR_UNIT_RIG
```mql5
CALENDAR_UNIT_RIG
```

---

### CALENDAR_UNIT_USD
```mql5
CALENDAR_UNIT_USD
```

---

### CALENDAR_UNIT_PEOPLE
```mql5
CALENDAR_UNIT_PEOPLE
```

---

### CALENDAR_UNIT_MORTGAGE
```mql5
CALENDAR_UNIT_MORTGAGE
```

---

### CALENDAR_UNIT_VOTE
```mql5
CALENDAR_UNIT_VOTE
```

---

### CALENDAR_UNIT_BARREL
```mql5
CALENDAR_UNIT_BARREL
```

---

### CALENDAR_UNIT_CUBICFEET
```mql5
CALENDAR_UNIT_CUBICFEET
```

---

### CALENDAR_UNIT_POSITION
```mql5
CALENDAR_UNIT_POSITION
```

---

### CALENDAR_UNIT_BUILDING
```mql5
CALENDAR_UNIT_BUILDING
```

---

### ENUM_CALENDAR_EVENT_MULTIPLIER
```mql5
ENUM_CALENDAR_EVENT_MULTIPLIER
```

---

### MULTIPLIER_NONE
```mql5
MULTIPLIER_NONE
```

---

### MULTIPLIER_THOUSANDS
```mql5
MULTIPLIER_THOUSANDS
```

---

### MULTIPLIER_MILLIONS
```mql5
MULTIPLIER_MILLIONS
```

---

### MULTIPLIER_BILLIONS
```mql5
MULTIPLIER_BILLIONS
```

---

### MULTIPLIER_TRILLIONS
```mql5
MULTIPLIER_TRILLIONS
```

---

### ENUM_CALENDAR_EVENT_IMPACT
```mql5
ENUM_CALENDAR_EVENT_IMPACT
```

---

### CALENDAR_IMPACT_NA
```mql5
CALENDAR_IMPACT_NA
```

---

### CALENDAR_IMPACT_POSITIVE
```mql5
CALENDAR_IMPACT_POSITIVE
```

---

### CALENDAR_IMPACT_NEGATIVE
```mql5
CALENDAR_IMPACT_NEGATIVE
```

---

### ENUM_CALENDAR_EVENT_TIMEMODE
```mql5
ENUM_CALENDAR_EVENT_TIMEMODE
```

---

### CALENDAR_TIMEMODE_DATETIME
```mql5
CALENDAR_TIMEMODE_DATETIME
```

---

### CALENDAR_TIMEMODE_DATE
```mql5
CALENDAR_TIMEMODE_DATE
```

---

### CALENDAR_TIMEMODE_NOTIME
```mql5
CALENDAR_TIMEMODE_NOTIME
```

---

### CALENDAR_TIMEMODE_TENTATIVE
```mql5
CALENDAR_TIMEMODE_TENTATIVE
```

---

### Alert
<void> Displays a message in a separate window.

```mql5
Alert(argument, ...)
```

---

### CheckPointer
```mql5
CheckPointer(object* anyobject)
```

---

### Comment
<void> outputs a comment defined by a user in the top left corner of a chart.

```mql5
Comment(argument, ...)
```

---

### CryptEncode
```mql5
CryptEncode(ENUM_CRYPT_METHOD method, const uchar& data[], const uchar& key[], uchar& result[])
```

---

### CryptEncode2
```mql5
CryptEncode(ENUM_CRYPT_METHOD method, const uchar& data[], const uchar& key[], uchar& result[])
```

---

### DebugBreak
<void> sets a debug break point

```mql5
DebugBreak()
```

---

### ExpertRemove
<void> stops an Expert Advisor and unloads it from a chart.

```mql5
ExpertRemove()
```

---

### GetPointer
<void*> returns the object pointer.

```mql5
GetPointer(object anytype)
```

---

### GetTickCount
<uint> returns the number of milliseconds that elapsed since the system start

```mql5
GetTickCount()
```

---

### GetTickCount64
```mql5
GetTickCount64()
```

---

### GetMicrosecondCount
<ulong> returns the number of microseconds that have elapsed since the start of MQL5-program.

```mql5
GetMicrosecondCount()
```

---

### MessageBox
<int> creates and shows a message box and manages it..

```mql5
MessageBox(string  text, caption=NULL, int flags)
```

---

### PeriodSeconds
<int> number of seconds in a period.

```mql5
PeriodSeconds(ENUM_TIMEFRAMES=PERIOD_CURRENT)
```

---

### PlaySound
<bool> plays a sound file.

```mql5
PlaySound(string  filename)
```

---

### Print
<void> enters a message in the Expert Advisor log. Parameters can be of any type.

```mql5
Print(argument, ...)
```

---

### PrintFormat
<void> formats and enters sets of symbols and values in the Expert Advisor log in accordance with a preset format.

```mql5
PrintFormat(string format_string,  ...)
```

---

### ResetLastError
<void> Sets the value of the predefined variable _LastError into zero.

```mql5
ResetLastError()
```

---

### ResourceCreate
```mql5
ResourceCreate(const string resource_name, const string path)
```

---

### ResourceFree
```mql5
ResourceFree(const string resource_name)
```

---

### ResourceReadImage
```mql5
ResourceReadImage(const string resource_name, uint& data[], uint& width, uint& height)
```

---

### ResourceSave
```mql5
ResourceSave(const string resource_name, const string file_name)
```

---

### SetUserError
```mql5
SetUserError(ushort user_error)
```

---

### SetReturnError
```mql5
SetReturnError(int ret_code)
```

---

### Sleep
<void> The function suspends execution of the current Expert Advisor or script within a specified interval.

```mql5
Sleep(int milliseconds)
```

---

### TerminalClose
```mql5
TerminalClose(int ret_code)
```

---

### TesterHideIndicators
```mql5
TesterHideIndicators(bool hide)
```

---

### TesterStatistics
```mql5
TesterStatistics(ENUM_STATISTICS statistic_id)
```

---

### TesterStop
```mql5
TesterStop()
```

---

### TesterDeposit
```mql5
TesterDeposit(double money)
```

---

### TesterWithdrawal
```mql5
TesterWithdrawal(double money)
```

---

### TranslateKey
<short> Returns a Unicode character by a virtual key code considering the current input language and the status of control keys.

```mql5
TranslateKey(int key_code)
```

---

### ZeroMemory
<void> resets a variable passed to it by reference.

```mql5
ZeroMemory(void &variable)
```

---

### ArrayBsearch
```mql5
ArrayBsearch(const double& array[], double value)
```

---

### ArrayBsearch2
```mql5
ArrayBsearch(const float& array[], float value)
```

---

### ArrayBsearch3
```mql5
ArrayBsearch(const long& array[], long value)
```

---

### ArrayBsearch4
```mql5
ArrayBsearch(const int& array[], int value)
```

---

### ArrayBsearch5
```mql5
ArrayBsearch(const short& array[], short value)
```

---

### ArrayBsearch6
```mql5
ArrayBsearch(const char& array[], char value)
```

---

### ArrayCopy
```mql5
ArrayCopy(void& dst_array[], const void& src_array[], int dst_start=0, int src_start=0, int count=WHOLE_ARRAY)
```

---

### ArrayCompare
```mql5
ArrayCompare(const void& array1[], const void& array2[], int start1=0, int start2=0, int count=WHOLE_ARRAY)
```

---

### ArrayFree
```mql5
ArrayFree(void& array[])
```

---

### ArrayGetAsSeries
<bool> It checks direction of an array index..

```mql5
ArrayGetAsSeries(const void& array[])
```

---

### ArrayInitialize
<int> initializes a numeric array by a preset value.

```mql5
ArrayInitialize(T array[], T value)
```

---

### ArrayInitialize2
```mql5
ArrayInitialize(short array[], short value)
```

---

### ArrayInitialize3
```mql5
ArrayInitialize(int array[], int value)
```

---

### ArrayInitialize4
```mql5
ArrayInitialize(long array[], long value)
```

---

### ArrayInitialize5
```mql5
ArrayInitialize(float array[], float value)
```

---

### ArrayInitialize6
```mql5
ArrayInitialize(double array[], double value)
```

---

### ArrayInitialize7
```mql5
ArrayInitialize(bool array[], bool value)
```

---

### ArrayInitialize8
```mql5
ArrayInitialize(uint array[], uint value)
```

---

### ArrayFill
```mql5
ArrayFill(void& array[], int start, int count, void value)
```

---

### ArrayIsSeries
```mql5
ArrayIsSeries(const void& array[])
```

---

### ArrayIsDynamic
```mql5
ArrayIsDynamic(const void& array[])
```

---

### ArrayMaximum
```mql5
ArrayMaximum(const void& array[], int start=0, int count=WHOLE_ARRAY)
```

---

### ArrayMinimum
```mql5
ArrayMinimum(const void& array[], int start=0, int count=WHOLE_ARRAY)
```

---

### ArrayPrint
```mql5
ArrayPrint(const void& array[], uint digits=_Digits, const string separator=NULL, ulong start=0, ulong count=WHOLE_ARRAY, ulong flags=ARRAYPRINT_HEADER|ARRAYPRINT_INDEX|ARRAYPRINT_LIMIT|ARRAYPRINT_ALIGN)
```

---

### ArrayRange
```mql5
ArrayRange(const void& array[], int rank_index)
```

---

### ArrayResize
<int> The function sets a new size for the first dimension

```mql5
ArrayResize(void& array[], int new_size,reserved_size=0)
```

---

### ArrayInsert
```mql5
ArrayInsert(void& dst_array[], const void& src_array[], uint dst_start, uint src_start=0, uint count=WHOLE_ARRAY)
```

---

### ArrayRemove
```mql5
ArrayRemove(void& array[], uint start, uint count=WHOLE_ARRAY)
```

---

### ArrayReverse
```mql5
ArrayReverse(void& array[], uint start=0, uint count=WHOLE_ARRAY)
```

---

### ArraySetAsSeries
<bool> The function sets the AS_SERIES flag to a selected object of a dynamic array, and elements will be indexed like in timeseries.

```mql5
ArraySetAsSeries(const void& array[], ${bool flag})
```

---

### ArraySize
<int> The function returns the number of elements of a selected array..

```mql5
ArraySize(const void& array[])
```

---

### ArraySort
```mql5
ArraySort(void& array[])
```

---

### ArraySwap
```mql5
ArraySwap(void& array1[], void& array2[])
```

---

### CharToString
<tostring> Converting a symbol code into a one-character string.

```mql5
CharToString(uchar char_code)
```

---

### DoubleToString
<string> Converting numeric value into text string.

```mql5
DoubleToString(double value, int digits=8)
```

---

### EnumToString
<string> Converting an enumeration value of any type to a text form.

```mql5
EnumToString(any_enum value)
```

---

### NormalizeDouble
<double> Rounding floating point number to a specified accuracy.

```mql5
NormalizeDouble(double value, int digits)
```

---

### StringToDouble
```mql5
StringToDouble(string value)
```

---

### StringToInteger
```mql5
StringToInteger(string value)
```

---

### StringToTime
<datetime> converts a string containing time or date in yyyy.mm.dd [hh:mi] format into datetime type.

```mql5
StringToTime(string value)
```

---

### TimeToString
<string> Converting a value containing time in seconds elapsed since 01.01.1970 into a string of yyyy.mm.dd hh:mi format.

```mql5
TimeToString(datetime value, int mode=TIME_DATE|TIME_MINUTES)
```

---

### IntegerToString
```mql5
IntegerToString(long number, int str_len=0, ushort fill_symbol=' ')
```

---

### ShortToString
```mql5
ShortToString(ushort symbol_code)
```

---

### ShortArrayToString
```mql5
ShortArrayToString(ushort array[], int start=0, int count=-1)
```

---

### StringToShortArray
```mql5
StringToShortArray(string text_string, ushort& array[], int start=0, int count=-1)
```

---

### CharArrayToString
<string> It copies and converts part of array of uchar type into a returned string..

```mql5
CharArrayToString(uchar array[], int start, int count=1, uint code_page=CP_ACP)
```

---

### StringToCharArray
<int> Symbol-wise copies a string converted from Unicode to ANSI, to a selected place of array of uchar type. It returns the number of copied elements.

```mql5
StringToCharArray(string text_string, uchar& array[], int start=0, int count=-1, uint codepage=CP_ACP)
```

---

### CharArrayToStruct
```mql5
CharArrayToStruct(void& struct_object, const uchar& char_array[], uint start_pos=0)
```

---

### StructToCharArray
```mql5
StructToCharArray(const void& struct_object, uchar& char_array[], uint start_pos=0)
```

---

### ColorToARGB
```mql5
ColorToARGB(color clr, uchar alpha=255)
```

---

### ColorToString
<string> It converts color value into string of R,G,B form.

```mql5
ColorToString(color color, bool show_color_name)
```

---

### StringToColor
```mql5
StringToColor(string color_string)
```

---

### StringFormat
<string> The function formats obtained parameters and returns a string.

```mql5
StringFormat(string format, params...)
```

---

### CalendarCountryById
```mql5
CalendarCountryById(const long country_id, MqlCalendarCountry& country)
```

---

### CalendarEventById
```mql5
CalendarEventById(ulong event_id, MqlCalendarEvent& event)
```

---

### CalendarValueById
```mql5
CalendarValueById(ulong value_id, MqlCalendarValue& value)
```

---

### CalendarCountries
```mql5
CalendarCountries(MqlCalendarCountry& countries[])
```

---

### CalendarEventByCountry
```mql5
CalendarEventByCountry(string country_code, MqlCalendarEvent& events[])
```

---

### CalendarEventByCurrency
```mql5
CalendarEventByCurrency(const string currency, MqlCalendarEvent& events[])
```

---

### CalendarValueHistoryByEvent
```mql5
CalendarValueHistoryByEvent(ulong event_id, MqlCalendarValue& values[], datetime datetime_from, datetime datetime_to=0)
```

---

### CalendarValueHistory
```mql5
CalendarValueHistory(MqlCalendarValue& values[], datetime datetime_from, datetime datetime_to=0, const string country_code=NULL, const string currency=NULL)
```

---

### CalendarValueLastByEvent
```mql5
CalendarValueLastByEvent(ulong event_id, ulong& change_id, MqlCalendarValue& values[])
```

---

### CalendarValueLast
```mql5
CalendarValueLast(ulong& change_id, MqlCalendarValue& values[], const string country_code=NULL, const string currency=NULL)
```

---

### SignalBaseGetDouble
```mql5
SignalBaseGetDouble(ENUM_SIGNAL_BASE_DOUBLE property_id)
```

---

### SignalBaseGetInteger
```mql5
SignalBaseGetInteger(ENUM_SIGNAL_BASE_INTEGER property_id)
```

---

### SignalBaseGetString
```mql5
SignalBaseGetString(ENUM_SIGNAL_BASE_STRING property_id)
```

---

### SignalBaseSelect
```mql5
SignalBaseSelect(int index)
```

---

### SignalBaseTotal
```mql5
SignalBaseTotal()
```

---

### SignalInfoGetDouble
```mql5
SignalInfoGetDouble(ENUM_SIGNAL_INFO_DOUBLE property_id)
```

---

### SignalInfoGetInteger
```mql5
SignalInfoGetInteger(ENUM_SIGNAL_INFO_INTEGER property_id)
```

---

### SignalInfoGetString
```mql5
SignalInfoGetString(ENUM_SIGNAL_INFO_STRING property_id)
```

---

### SignalInfoSetDouble
```mql5
SignalInfoSetDouble(ENUM_SIGNAL_INFO_DOUBLE property_id, double value)
```

---

### SignalInfoSetInteger
```mql5
SignalInfoSetInteger(ENUM_SIGNAL_INFO_INTEGER property_id, long value)
```

---

### SignalSubscribe
```mql5
SignalSubscribe(long signal_id)
```

---

### SignalUnsubscribe
```mql5
SignalUnsubscribe()
```

---

### datetime
```mql5
datetime
```

---

### color
```mql5
color
```

---

### ulong
```mql5
ulong
```

---

### ushort
```mql5
ushort
```

---

### uchar
```mql5
uchar
```

---

### uint
```mql5
uint
```

---

### string
```mql5
string
```

---

### NULL
```mql5
NULL
```

---

### include
preprocessor include directive

```mql5
#include <file_name.mqh>
```

---

### dynamic_cast
['Dynamic typecasting is performed using dynamic_cast operator that can be applied only to pointers to classes.', 'Type validation is performed at runtime. This means that the compiler does not check the data type applied for typecasting when dynamic_cast operator is used.', 'If a pointer is converted to a data type which is not the actual type of an object, the result is NULL.']

```mql5
dynamic_cast<type-id>(expression)
```

---

### OP_BUY
```mql5
OP_BUY
```

---

### OP_BUYLIMIT
```mql5
OP_BUYLIMIT
```

---

### OP_BUYSTOP
```mql5
OP_BUYSTOP
```

---

### OP_SELL
```mql5
OP_SELL
```

---

### OP_SELLLIMIT
```mql5
OP_SELLLIMIT
```

---

### OP_SELLSTOP
```mql5
OP_SELLSTOP
```

---

### MqlDateTime
<struct> structure contains eight fields of the int type

```mql5
MqlDateTime 
```

---

### MqlParam
<struct> The MqlParam structure has been specially designed to provide input parameters when creating the handle of a technical indicator using the IndicatorCreate() function.

```mql5
MqlParam 
```

---

### MqlRates
<struct> structure stores information about the prices, volumes and spread.

```mql5
MqlRates 
```

---

### MqlBookInfo
<struct> provides information about the market depth data

```mql5
MqlBookInfo 
```

---

### MqlTradeRequest
<struct> Interaction between the client terminal and a trade server for executing the order placing operation is performed by using trade requests. 

```mql5
MqlTradeRequest 
```

---

### MqlTradeCheckResult
<struct> Before sending a request for a trade operation to a trade server, it is recommended to check it. The check is performed using the OrderCheck() function, to which the checked request and a variable of the MqlTradeCheckResult structure type are passed. The check result will be written to this variable.

```mql5
MqlTradeCheckResult 
```

---

### MqlTradeResult
<struct> As result of a trade request, a trade server returns data about the trade request processing result as a special predefined structure of MqlTradeResult type.

```mql5
MqlTradeResult 
```

---

### MqlTick
<struct> This is a structure for storing the latest prices of the symbol. It is designed for fast retrieval of the most requested information about current prices.

```mql5
MqlTick 
```

---

### _Symbol
<string> Returns the string value of the current symbol.

```mql5
_Symbol
```

---

### _Digits
<int> Number of decimal places

```mql5
_Digits
```

---

### _Point
<double> Size of the current symbol point in the quote currency

```mql5
_Point
```

---

### _LastError
<int> last error code

```mql5
_LastError
```

---

### _Period
<ENUM_TIMEFRAMES> value of the timeframe of the current chart.

```mql5
_Period
```

---

### _RandomSeed
<int> Variable for storing the current state when generating pseudo-random integers

```mql5
_RandomSeed
```

---

### _StopFlag
<bool> contains the flag of the mql5-program stop

```mql5
_StopFlag
```

---

### _UninitReason
<int> contains the code of the program uninitialization reason.

```mql5
_UninitReason
```

---

### _AppliedTo
```mql5
_AppliedTo
```

---

### _IsX64
```mql5
_IsX64
```

---

### Check Pointer
<ENUM_POINTER_TYPE> The function returns the type of the object pointer.

```mql5
CheckPointer(object* anytype)
```

---

### SendNotification
<bool> Sends push notifications to the mobile terminals, whose MetaQuotes IDs are specified in the "Notifications" tab..

```mql5
SendNotification(string text)
```

---

### SendMail
<bool> Sends an email at the address specified in the settings window of the Email tab.

```mql5
SendMail(string subject, string text)
```

---

### WebRequest
<int> sends an HTTP request to a specified server. The function has two versions:

```mql5
WebRequest(see docs)
```

---

### TimeCurrentStruct
<datetime> MqlDateTime structure type variable has been passed as a parameter, it is filled accordingly

```mql5
TimeCurrent(MqlDateTime struct)
```

---

### TimeCurrent
<datetime> Returns the last known server time

```mql5
TimeCurrent()
```

---

### TimeTradeServer
<datetime> Returns the calculated current time of the trade server

```mql5
TimeTradeServer()
```

---

### TimeLocal
<datetime> Returns the local time of a computer

```mql5
TimeLocal()
```

---

### TimeLocal Struct
<datetime> Returns the local time of a computer; fills struct

```mql5
TimeLocal(MqlDateTime &struct)
```

---

### TimeGMT
<datetime> Returns the GMT, which is calculated taking into account the DST switch by the local time on the computer where the client terminal is running.

```mql5
TimeGMT()
```

---

### TimeGMT Struct
<datetime> Returns the GMT, which is calculated taking into account the DST switch by the local time on the computer where the client terminal is running.

```mql5
TimeGMT(MqlDateTime &struct)
```

---

### TimeDaylightSavings
<datetime> Returns correction for daylight saving time in seconds, if the switch to summer time has been made.

```mql5
TimeDaylightSavings()
```

---

### TimeGMTOffset
<datetime> Returns the current difference between GMT time and the local computer time in seconds

```mql5
TimeGMTOffset()
```

---

### TimeToStruct
<bool> Converts a value of datetime type (number of seconds since 01.01.1970) into a structure variable MqlDateTime.

```mql5
TimeToStruct(datetime dt, MqlDateTime &struct)
```

---

### StructToTime
<datetime> Converts a structure variable MqlDateTime into a value of datetime type and returns the resulting value.

```mql5
StructToTime(MqlDateTime &struct)
```

---

### StringAdd
<bool> adds a substring to the end of a string.

```mql5
StringAdd(string& str_var, string add_substring)
```

---

### StringBufferLen
<int> returns the size of buffer allocated for the string.

```mql5
StringBufferLen(string string_var)
```

---

### StringCompare
<int> compares two strings and returns the comparison result in form of an integer.Case sensitivity mode selection. If it is true, then A>a. If it is false, then A=a.

```mql5
StringCompare(string str1, string str2,${bool case_sensitive=true})
```

---

### StringFill
<bool> It fills out a selected string by specified symbols

```mql5
StringFill(string& str_var, ushort character)
```

---

### StringFind
<int> Search for a substring in a string.

```mql5
StringFind(string value, string match_substring,int start_pos=0)
```

---

### StringGetCharacter
<ushort> returns value of a symbol, located in the specified position of a string.

```mql5
StringGetCharacter(string str_var, int pos)
```

---

### StringLen
<int> Returns the number of symbols in a string

```mql5
StringLen(string str_var)
```

---

### StringReplace
['<int> replaces all the found substrings of a string by a set sequence of symbols.', 'The function returns the number of replacements in case of success, otherwise -1. To get an error code call the GetLastError() function.']

```mql5
StringReplace(string& str, string find, string replace)
```

---

### StringSplit
<int> Gets substrings by a specified separator from the specified string, returns the number of substrings obtained.

```mql5
StringSplit(string str, ushort separator, string &result[])
```

---

### StringSubstr
<string> Extracts a substring from a text string starting from the specified position.

```mql5
StringSubstr(string str, int start_pos, ${3:int length=-1)
```

---

### StringToLower
<bool> Transforms all symbols of a selected string into lowercase.

```mql5
StringToLower(string& str)
```

---

### StringToUpper
<bool> Transforms all symbols of a selected string into capitals.

```mql5
StringToUpper(string& str)
```

---

### StringTrimRight
<int> The function cuts line feed characters, spaces and tabs in the right part of the string after the last meaningful symbol. The string is modified at place.

```mql5
StringTrimRight(string& str)
```

---

### StringTrimLeft
<int> The function cuts line feed characters, spaces and tabs in the left part of the string till the first meaningful symbol. The string is modified at place.

```mql5
StringTrimLeft(string& str)
```

---

### AccountInfoDouble
<double> Returns the value of the corresponding account property.

```mql5
AccountInfoDouble(ENUM_ACOUNT_INFO_DOUBLE property_id)
```

---

### AccountInfoInteger
<long> Returns the value of the corresponding account property.

```mql5
AccountInfoInteger(ENUM_ACOUNT_INFO_INTEGER  property_id)
```

---

### AccountInfoString
<string> Returns the value of the corresponding account property.

```mql5
AccountInfoString(ENUM_ACOUNT_INFO_STRING  property_id)
```

---

### GetLastError
<int> Returns the contents of the system variable _LastError

```mql5
GetLastError()
```

---

### IsStopped
<bool> Checks the forced shutdown of an mql5 program

```mql5
IsStopped()
```

---

### UninitializeReason
<int> Returns the code of a reason for deinitialization.

```mql5
UninitializeReason()
```

---

### TerminalInfoInteger
<long> Returns the value of a corresponding property of the mql5 program environment

```mql5
TerminalInfoInteger(int property_id)
```

---

### TerminalInfoDouble
<double> Returns the value of a corresponding property of the mql5 program environment

```mql5
TerminalInfoDouble(int property_id)
```

---

### TerminalInfoString
<string> Returns the value of a corresponding property of the mql5 program environment

```mql5
TerminalInfoString(int property_id)
```

---

### MQLInfoInteger
<int> Returns the value of a corresponding property of a running mql5 program.

```mql5
MQLInfoInteger(int property_id)
```

---

### MQLInfoString
<string> Returns the value of a corresponding property of a running mql5 program.

```mql5
MQLInfoString(int property_id)
```

---

### SymbolsTotal
<int> Returns the number of available (selected in Market Watch or all) symbols.

```mql5
SymbolsTotal(bool selected)
```

---

### SymbolName
<string> returns the name of the symbol from the marketwatch window.

```mql5
SymbolName(int pos, bool selected)
```

---

### SymbolSelect
<bool> Selects a symbol in the Market Watch window or removes a symbol from the window.

```mql5
SymbolSelect(string name, bool select)
```

---

### SymbolIsSynchronized
<bool> The function checks whether data of a selected symbol in the terminal are synchronized with data on the trade server.

```mql5
SymbolIsSynchronized(string name)
```

---

### SymbolInfoTick
<bool> returns current prices of a specified symbol in a variable of the MqlTick type.

```mql5
SymbolInfoTick(string name, MqlTick& tick)
```

---

### MarketBookAdd
<bool> Provides opening of Depth of Market for a selected symbol, and subscribes for receiving notifications of the DOM changes.

```mql5
MarketBookAdd(string name)
```

---

### MarketBookRelease
<bool> Provides closing of Depth of Market for a selected symbol, and cancels the subscription for receiving notifications of the DOM changes.

```mql5
MarketBookRelease(string name)
```

---

### MarketBookGet
<bool> Returns a structure array MqlBookInfo containing records of the Depth of Market of a specified symbol.

```mql5
MarketBookGet(string name, MqlBookInfo&  book[])
```

---

### SymbolInfoInteger
<long> Returns the corresponding property of a specified symbol.

```mql5
SymbolInfoInteger(string name, ENUM_SYMBOL_INFO_STRING prop_id)
```

---

### SymbolInfoString
<string> Returns the corresponding property of a specified symbol.

```mql5
SymbolInfoString(string name, ENUM_SYMBOL_INFO_INTEGER prop_id)
```

---

### SymbolInfoDouble
<double> Returns the corresponding property of a specified symbol.

```mql5
SymbolInfoDouble(string name, ENUM_SYMBOL_INFO_DOUBLE prop_id)
```

---

### Bars_From_To
<int> Returns the number of bars count in the history for a specified symbol and period.

```mql5
Bars(string name, ENUM_TIMEFRAMES timeframe, datetime start_time, datetime stop_time)
```

---

### Bars
<int> Returns the number of bars count in the history for a specified symbol and period.

```mql5
Bars(string name, ENUM_TIMEFRAMES timeframe)
```

---

### BarsCalculated
<int> Returns the number of calculated data for the specified indicator

```mql5
BarsCalculated(int ind_handle)
```

---

### IndicatorRelease
<bool> removes an indicator handle and releases the calculation block of the indicator, if it's not used by anyone else.

```mql5
IndicatorRelease(int ind_handle)
```

---

### CopyTicks
<int> receives ticks in the MqlTick format into ticks_array.

```mql5
CopyTicks(string symbol, MqlTick& tickarray[], uint flags=COPY_TICKS_ALL, ulong from=0, uint count=0)
```

---

### CopyBuffer
<int> Gets data of a specified buffer of a certain indicator in the necessary quantity.

```mql5
CopyBuffer(int handle, int buffer_number, int start_pos|datetime start_time, int count|datetime stop_time, double buffer[])
```

---

### CopyRates
<int> Gets history data of MqlRates structure of a specified symbol-period in specified quantity into the rates_array array. The elements ordering of the copied data is from present to the past, i.e., starting position of 0 means the current bar.

```mql5
CopyRates(string symbol, ENUM_TIMEFRAMES timeframe, int start_pos|datetime start_time, int count|datetime stop_time, MqlRates rates_array[])
```

---

### EventSetMillisecondTimer
<bool> indicates to the client terminal that timer events should be generated at intervals less than one second for this Expert Advisor or indicator.

```mql5
EventSetMillisecondTimer(int milliseconds)
```

---

### EventSetTimer
<bool> indicates to the client terminal, that for this indicator or Expert Advisor, events from the timer must be generated with the specified periodicity.

```mql5
EventSetTimer(int seconds)
```

---

### EventKillTimer
<bool> Specifies the client terminal that is necessary to stop the generation of events from Timer.

```mql5
EventKillTimer()
```

---

### EventChartCustom
<bool> The function generates a custom event for the specified chart.

```mql5
EventChartCustom()
```

---

### OrderClose
<bool> Closes opened order.

```mql5
OrderClose(int ticket, double lots, double price, int slippage, color arrow_color=clrNone)
```

---

### OrderCloseBy
<bool> Closes an opened order by another opposite opened order.

```mql5
OrderCloseBy(int ticket, int opposite, color arrow_color=clrNone)
```

---

### OrderClosePrice
<double> Returns close price of the currently selected order. If the order is live this will return the price of which it is to be closed.

```mql5
OrderClosePrice()
```

---

### OrderCloseTime
<datetime> Returns close time of the currently selected order.

```mql5
OrderCloseTime(int ticket, double lots, double price, int slippage, color arrow_color)
```

---

### OrderComment
<string> Returns comment of the currently selected order.

```mql5
OrderComment()
```

---

### OrderCommission
<double> Returns calculated commission of the currently selected order.

```mql5
OrderCommission()
```

---

### OrderDelete
<bool> Deletes previously opened pending order.

```mql5
OrderDelete(int ticket, color arrow_color=clrNone)
```

---

### OrderExpiration
<datetime> Returns expiration date of the selected pending order.

```mql5
OrderExpiration()
```

---

### OrderLots
<double> Returns amount of lots of the selected order.

```mql5
OrderLots()
```

---

### OrderMagicNumber
<int> Returns an identifying (magic) number of the currently selected order.

```mql5
OrderMagicNumber()
```

---

### OrderModify
<bool> Modification of characteristics of the previously opened or pending orders.

```mql5
OrderModify(int ticket, double price, double stoploss, double takeprofit, datetime expiration, color arrow_color=clrNone)
```

---

### OrderOpenPrice
<double> Returns open price of the currently selected order.

```mql5
OrderOpenPrice()
```

---

### OrderOpenTime
<datetime> Returns open time of the currently selected order.

```mql5
OrderOpenTime()
```

---

### OrderPrint
<void> Prints information about the selected order in the log.

```mql5
OrderPrint()
```

---

### OrderProfit
<double> Returns profit of the currently selected order.

```mql5
OrderProfit()
```

---

### OrdersHistoryTotal
<int> Returns the number of closed orders in the account history loaded into the terminal. 

```mql5
OrdersHistoryTotal)
```

---

### OrderStopLoss
<double> Returns stoploss of the currently selected order.

```mql5
OrderStopLoss(int ticket, double lots, double price, int slippage, color arrow_color)
```

---

### OrderSwap
<double> Returns swap value of the currently selected order.

```mql5
OrderSwap()
```

---

### OrderTakeProfit
<datetime> Returns take profit value of the currently selected order.

```mql5
OrderTakeProfit()
```

---

### OrderSymbol
<string> Returns symbol of the currently selected order.

```mql5
OrderSymbol()
```

---

### OrderTicket
<int> Returns order ticket number of the currently selected order.

```mql5
OrderTicket()
```

---

### OrderType
<int> Returns order operation type of the currently selected order. OP_BUY=buy-order, OP_SELL=sell-order, OP_BUYLIMIT=buy-limit, OP_BUYSTOP=buy-stop, OP_SELLLIMIT=sell-limit, OP_SELLSTOP=sell-stop.

```mql5
OrderType()
```

---

### for forward
mql4 orderselect loop

```mql5
for(int i=0;i < int max_iter;i++)
{
   
}
```

---

### for backward
mql4 orderselect loop

```mql5
for(int i=int max_iter - 1;i >= 0 ;i--)
{
   
}
```

---

### for OrdersTotal
mql4 orderselect loop

```mql5
for(int i=OrdersTotal()-1;i>=0;i--)
{
   if(OrderSelect(i,SELECT_BY_POS) && OrderSymbol() == _Symbol  other conditions)
   {
      
   }
}
```

---

### for OrdersHistoryTotal
mql4 orderselect loop

```mql5
for(int i=OrdersHistoryTotal()-1;i>=0;i--)
{
   if(OrderSelect(i,SELECT_BY_POS,MODE_HISTORY) && OrderSymbol() == _Symbol  other conditions)
   {
      
   }
}
```

---

### Script_Template
```mql5
//+------------------------------------------------------------------+
//| file_name.mq4.mq4
//| Copyright 2017, Author Name
//| Link
//+------------------------------------------------------------------+
#property copyright "Copyright 2017, Author Name"
#property link      "Link"
#property version   "1.00"
#property strict

 
 
void OnStart()
{
   
}

```

---

### Expert_Template
expert advisor template

```mql5
//+------------------------------------------------------------------+
//| file_name.mq4.mq4
//| Copyright 2017, Author Name
//| Link
//+------------------------------------------------------------------+
#property copyright "Copyright 2017, Author Name"
#property link      "Link"
#property version   "1.00"
#property strict

 
 
//+------------------------------------------------------------------+
//| Expert initialization function                                   |
//+------------------------------------------------------------------+
int OnInit()
{
   EventSetTimer(60);
   
   return(INIT_SUCCEEDED);
}
//+------------------------------------------------------------------+
//| Expert deinitialization function                                 |
//+------------------------------------------------------------------+
,void OnDeinit(const int reason)
{
 EventKillTimer();
    
}
//+------------------------------------------------------------------+
//| Expert tick function                                             |
//+------------------------------------------------------------------+
void OnTick()
{
   
}
//+------------------------------------------------------------------+
//| Timer function                                                   |
//+------------------------------------------------------------------+
void OnTimer()
{
  
}
//+------------------------------------------------------------------+
//| ChartEvent function                                              |
//+------------------------------------------------------------------+
void OnChartEvent(const int id,
                const long &lparam,
                const double &dparam,
                const string &sparam)
{
 
}
//+------------------------------------------------------------------+
```

---

### Function Header
```mql5
//+------------------------------------------------------------------+
//| type FuntionName : description
//+------------------------------------------------------------------+
type FunctionName()
{
   
}
```

---

