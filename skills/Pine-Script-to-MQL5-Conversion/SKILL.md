
Pine Script v5/v6 to MQL5 Conversion Skill

[TOC] Table of Contents

[SECTION_SUMMARY] The Golden Standard (Architectural Baseline)

[SECTION_STATE] Persistent State & Variable Emulation

[SECTION_MTF] Multi-Timeframe (MTF) & Security

[SECTION_EXECUTION] Strategy to EA Execution Gating

[SECTION_DATA] Data Structures & Collections Mapping

[SECTION_TRAPS] Silent Failures Checklist

[SECTION_RESOURCES] Links to Specialized References

[SECTION_SUMMARY] The Golden Standard

Для обеспечения 100% идентичности исполнения (Execution Parity) и отсутствия перерисовки (Non-Repainting), придерживайтесь следующих правил:

Deterministic State: Используйте static переменные внутри OnCalculate с защитой инициализации prev_calculated == 0.

Incremental Calculation: Всегда пересчитывайте только последний бар: int start = (prev_calculated > 0) ? prev_calculated - 1 : 0.

Array Direction: Принудительно устанавливайте ArraySetAsSeries(buffer, true) для всех ценовых массивов.

MTF Security: Используйте правило Shift + 1 для HTF-данных, чтобы исключить утечки из будущего (Future Leaks).

ECN Trade: Открывайте позицию без SL/TP, затем модифицируйте тикет (Protocol: Request -> Ticket -> Modify).

[SECTION_STATE] Persistent State & Variable Emulation

Замена функциональной модели Pine на императивную модель MQL5.

var (Historical): static + guard. Переменная сохраняет значение между барами.

varip (Intrabar): static + New Bar Detection. Значение обновляется каждый тик внутри бара.

Details: See references/State_Persistence.md for pattern implementations.

[SECTION_MTF] Multi-Timeframe (MTF) & Security

Критическая секция для предотвращения Repainting.

Logic: Синхронизация через iBarShift.

Security: Если LTF-бар еще не закрыт, мы НЕ имеем права брать данные HTF-бара с индексом [0].

Grep Pattern: HTF_Buffer[shift + 1]

Details: See references/MTF_Sync.md for synchronization logic.

[SECTION_EXECUTION] Strategy to EA Execution Gating

Перевод Pine Strategies в торговых советников (EA).

Timing: Pine исполняет ордер на Open следующего бара после сигнала.

MQL5 implementation: Используйте фильтр New Bar в OnTick, чтобы симулировать закрытие свечи.

Order Protocol: Использование класса CTrade из стандартной библиотеки.

Details: See references/Execution_Mapping.md for order mapping rules.

[SECTION_DATA] Data Structures & Collections Mapping

Перенос сложных типов данных из Pine v6.

UDT -> Class: Пользовательские типы маппятся в классы для поддержки инкапсуляции.

Map -> CHashMap: Использование #include <Generic\HashMap.mqh>.

Matrix -> Flat Array: Эмуляция через одномерный массив с макросом IDX(r,c).

Details: See references/Data_Collections.md for OOP patterns.

[SECTION_TRAPS] Silent Failures Checklist

Чек-лист перед компиляцией:

[ ] Все ли массивы проинициализированы ArraySetAsSeries?

[ ] Используется ли NormalizeDouble(price, _Digits) перед OrderSend?

[ ] Нет ли рекурсивных вызовов в циклах (O(N^2))?

[ ] Обработан ли na через MathIsValidNumber?

[SECTION_RESOURCES] Links to Specialized References

State Persistence Patterns

MTF Synchronization & Non-Repainting

Execution Engine & Trade Protocols

Data Structures & Matrices

Created by MQL5 AI-assisted Coding agent | Ref: ThomasPraun/mql-developer Standards
