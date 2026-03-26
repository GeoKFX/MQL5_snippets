[SKILL] Pine Script to MQL5 Conversion

name: PineScript-to-MQL5-Architect
description: Expert system for deterministic conversion of Pine Script v5/v6 to MQL5 with zero-repainting guarantees.
allowed-tools: [google_search, mql5_hot_base, canvas_artifacts]

TABLE OF CONTENTS

CORE_EXECUTION_STATE

DATA_STRUCTURE_MAPPING

MTF_SECURITY_ALIGNMENT

STRATEGY_EA_PARITY

SILENT_TRAPS_CHECKLIST

REFERENCE_DOCUMENTATION

## [CORE_EXECUTION_STATE]

This section handles the translation of Pine's vectorized execution into MQL5's event-driven state machine.

Rule 1.1 (var/varip): Replicate persistence using static variables. var requires a prev_calculated == 0 guard. varip requires manual "New Bar" detection to manage intrabar state.

Rule 1.2 (Looping): Implement incremental loops: int start = (prev_calculated > 0) ? prev_calculated - 1 : 0. Re-evaluating the current bar is mandatory for recursive integrity.

Rule 1.3 (Indexing): Enforce ArraySetAsSeries(true) to align MQL5 with Pine’s reverse-chronological indexing [0].

## [DATA_STRUCTURE_MAPPING]

Mapping functional Pine v6 structures to Object-Oriented MQL5.

Rule 2.1 (UDTs): Convert Pine type definitions to MQL5 class structures. Classes support methods and dynamic memory via CArrayObj.

Rule 2.2 (Collections): * Pine Map → CHashMap<K, V>.

Pine Matrix → Flattened 1D array with IDX(r, c) macro access.

Pine Array → CArrayDouble or native dynamic arrays.

## [MTF_SECURITY_ALIGNMENT]

Deterministic time alignment for request.security without future-leaks.

Rule 3.1 (Shift + 1 Rule): Use iBarShift to align LTF time to HTF index. Always access [shift + 1] for closed-bar data (lookahead_off parity).

Rule 3.2 (Sync Guard): Always validate iBarShift return values (!= -1) before data access.

## [STRATEGY_EA_PARITY]

Ensuring Pine backtest results match MQL5 Live Execution.

Rule 4.1 (Execution Gating): Use an IsNewBar() filter in OnTick() to mimic Pine's bar-close evaluation model.

Rule 4.2 (ECN Protocol): Follow the "Open-then-Modify" sequence: trade.Buy() -> ResultOrder() -> trade.PositionModify().

Rule 4.3 (Pyramiding): Manually track position counts using PositionsTotal() filtered by Magic Number and Symbol.

## [SILENT_TRAPS_CHECKLIST]

Critical checks to prevent logic corruption.

[TRAP_1] Floating Point Drift: Normalize all prices to _Digits.

[TRAP_2] Recursive Drift: Ensure incremental calculation for EMA/RMA.

[TRAP_3] Implicit NaN: Use MathIsValidNumber() to mimic Pine's na propagation.

[TRAP_4] Array Direction Consistency: Mixing series and non-series indices leads to signal inversion.

[TRAP_5] Integer Division: Pine 5/2 = 2.5, MQL5 5/2 = 2. Use explicit casting (double)x/y.

## [REFERENCE_DOCUMENTATION]

For detailed implementation patterns and ready-to-use code snippets, refer to:

Snippets Library: A comprehensive collection of MQL5 code fragments for state persistence, MTF handling, and ECN-compatible trading.
