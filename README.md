---



```markdown
# MQL5 Snippets & Agentic Skills Library

Welcome to the central MQL5 knowledge base designed specifically for **AI-assisted algorithmic trading development**.

This repository serves as a strict syntactical and algorithmic reference to prevent AI hallucinations, enforce correct MQL5 architecture, and ensure highly efficient, production-ready code generation.

## 🧬 Repository Structure

The knowledge base is divided into two primary categories: **Skills** (AI operational directives and patterns) and **Snippets** (Raw code templates and logic).

### 🧠 1. Agentic Skills (`/skills`)

This directory contains context-rich Markdown files designed to act as "Skills" or "System Prompts" for AI agents. They provide battle-tested architectural patterns and troubleshooting checklists for specific MQL5 tasks.

* [**Pine Script to MQL5 Conversion**](skills/Pine-Script-to-MQL5-Conversion/SKILL.md)
  * **Purpose:** Expert system for deterministic conversion of Pine Script v5/v6 to MQL5 with zero-repainting guarantees.
  * **Key Concepts:** Execution state management (`var`/`varip` replication), incremental looping efficiency, data structure mapping (UDTs to classes), MTF security alignment (Shift + 1 rule), and EA execution parity.
  * **References:** Includes a comprehensive [Pine to MQL5 Snippets Library](skills/Pine-Script-to-MQL5-Conversion/references/Pine-to-MQL5_Snippets_library.md) providing production-ready code fragments for persistence, data synchronization, and ECN-compatible trading.

* [**MQL5 Visual Indicator Patterns**](skills/mql5-indicator-patterns/SKILL.md) 
  * **Purpose:** Essential patterns for creating custom indicators, managing buffers, and handling real-time chart updates without visual drift.
  * **Key Concepts:** Visible vs. Hidden buffer architecture, explicit display scaling for small values (`< 1.0`), new bar detection (to prevent rolling window drift), and correct `PLOT_DRAW_BEGIN` warmup calculations.
  * **References:** Includes deep-dives on [Buffer Patterns](skills/mql5-indicator-patterns/references/buffer-patterns.md), [Display Scaling](skills/mql5-indicator-patterns/references/display-scale.md), [Recalculation](skills/mql5-indicator-patterns/references/recalculation.md), and a [Complete Working Template](skills/mql5-indicator-patterns/references/complete-template.md).

### 🗃️ 2. Hot Codebase & Snippets (`/snippets`)

This section contains ready-to-use templates, functions, enumerations, and custom algorithms.

* [**Advanced Logic Snippets**](snippets/mq5%20advanced_logic%20snippets.md)
  * Complex algorithmic solutions including: Broker GMT Offset calculation, precise Lot Size calculation (Margin per Micro Lot), Trading Hours Filters (with day-of-week checks), Candlestick Pattern detection, and Strategy Tester speed throttling.

* [**MQL5 Standard Snippets**](snippets/mq5-snippets.md)
  * Quick-insert templates for MT5 specific functions (`iMACD`, `iStochastic`, `iMA`), graphical object creation (`OBJ_TEXT`, `OBJ_RECTANGLE_LABEL`, `OBJ_TREND`), and stream/buffer setup.

* [**MQL5 Core Snippets Base**](snippets/MQL5%20Snippets.md)
  * Massive dictionary of standard MQL5 event handlers (`OnInit`, `OnTick`, `OnCalculate`, etc.), trade functions, math functions, file operations, and terminal info calls.

* [**MQL4/MQL5 Core Snippets (English Reference)**](snippets/mql4%20mql5%20Snippets_en.md)
  * Extensive cross-reference library for standard constants, enumerations (`ENUM_TIMEFRAMES`, `ENUM_MA_METHOD`), and standard library function definitions.

* [**Nicholas Barker MQL4/MQL5 Library**](snippets/nicholishen%20Nicholas%20Barker%20MQL4%20MQL5%20Snippets.md)
  * Additional specific implementations and helper definitions.

### 📚 3. Guides & Optimization References

*In addition to raw code, this knowledge base incorporates core principles from essential MQL5 developer guides:*

* **HUD Implementation:** Best practices for creating a custom Heads-Up Display using `Comment()` or graphical objects to track EA state, PnL, margin, and order send execution times.

* **Execution Frequency (`OnTick` vs `OnTimer`):** Architectural guidance on when to use `OnTick()` (for immediate price responsiveness) versus `OnTimer()` (for CPU load management, multi-symbol handling, and time-based logic).

* **Code Profiling & Speed Optimization:** Techniques for using the MetaEditor Profiler to identify bottlenecks (`Self CPU %`), caching static data (like `MarketInfo` inside `OnInit()`), and optimizing loops.

* **Debugging:** Steps for effectively using the MT4/MT5 debugger, stepping through code, and using the Watch Window to squash logic bugs.

---

## 🤖 Directives for AI Agents

**MANDATORY PROTOCOL:** Before generating any MQL5 solutions, the AI Agent MUST:

1. **Consult the Skills Directory:** If the task involves indicators, UI, or specific architectural patterns, explicitly read the associated `SKILL.md` and its references first.

2. **Verify Syntax:** Cross-reference any standard MQL5 functions with the `snippets/` database to ensure strict adherence to MQL5 standard libraries (e.g., using `CTrade` or correct `OrderSend` structures).

3. **Prioritize Efficiency:** Always apply optimization principles — calculate data only once per bar where possible, cache static variables in `OnInit()`, and strictly manage arrays with `ArraySetAsSeries(..., false)` when forward-indexing is required.
