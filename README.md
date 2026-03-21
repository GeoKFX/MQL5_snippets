MQL5 Snippets & Agentic Skills Library

Welcome to the central MQL5 knowledge base designed specifically for AI-assisted algorithmic trading development.

This repository serves as a strict syntactical and algorithmic reference to prevent AI hallucinations, enforce correct MQL5 architecture, and ensure highly efficient, production-ready code generation.

🗂 Repository Structure

The knowledge base is divided into two primary categories: Skills (AI operational directives and patterns) and Snippets (Raw code templates and logic).

🧠 1. Agentic Skills (/skills)

This directory contains context-rich Markdown files designed to act as "Skills" or "System Prompts" for AI agents. They provide battle-tested architectural patterns and troubleshooting checklists for specific MQL5 tasks.

MQL5 Visual Indicator Patterns * Purpose: Essential patterns for creating custom indicators, managing buffers, and handling real-time chart updates without visual drift.

Key Concepts: Visible vs. Hidden buffer architecture, explicit display scaling for small values (< 1.0), new bar detection (to prevent rolling window drift), and correct PLOT_DRAW_BEGIN warmup calculations.

References: Includes deep-dives on Buffer Patterns, Display Scaling, Recalculation, and a Complete Working Template.

🔥 2. Hot Codebase & Snippets (/snippets)

This section contains ready-to-use templates, functions, enumerations, and custom algorithms.

Advanced Logic Snippets

Complex algorithmic solutions including: Broker GMT Offset calculation, precise Lot Size calculation (Margin per Micro Lot), Trading Hours Filters (with day-of-week checks), Candlestick Pattern detection, and Strategy Tester speed throttling.

MQL5 Standard Snippets

Quick-insert templates for MT5 specific functions (iMACD, iStochastic, iMA), graphical object creation (OBJ_TEXT, OBJ_RECTANGLE_LABEL, OBJ_TREND), and stream/buffer setup.

MQL5 Core Snippets Base

Massive dictionary of standard MQL5 event handlers (OnInit, OnTick, OnCalculate, etc.), trade functions, math functions, file operations, and terminal info calls.

MQL4/MQL5 Core Snippets (English Reference)

Extensive cross-reference library for standard constants, enumerations (ENUM_TIMEFRAMES, ENUM_MA_METHOD), and standard library function definitions.

Nicholas Barker MQL4/MQL5 Library

Additional specific implementations and helper definitions.

📚 3. Guides & Optimization References

In addition to raw code, this knowledge base incorporates core principles from essential MQL5 developer guides:

HUD Implementation: Best practices for creating a custom Heads-Up Display using Comment() or graphical objects to track EA state, PnL, margin, and order send execution times.

Execution Frequency (OnTick vs OnTimer): Architectural guidance on when to use OnTick() (for immediate price responsiveness) versus OnTimer() (for CPU load management, multi-symbol handling, and time-based logic).

Code Profiling & Speed Optimization: Techniques for using the MetaEditor Profiler to identify bottlenecks (Self CPU %), caching static data (like MarketInfo inside OnInit()), and optimizing loops.

Debugging: Steps for effectively using the MT4/MT5 debugger, stepping through code, and using the Watch Window to squash logic bugs.

🤖 Directives for AI Agents

MANDATORY PROTOCOL: Before generating any MQL5 solutions, the AI Agent MUST:

Consult the Skills Directory: If the task involves indicators, UI, or specific architectural patterns, explicitly read the associated Skill.md and its references first.

Verify Syntax: Cross-reference any standard MQL5 functions with the snippets/ database to ensure strict adherence to MQL5 standard libraries (e.g., using CTrade or correct OrderSend structures).

Prioritize Efficiency: Always apply optimization principles—calculate data only once per bar where possible, cache static variables in OnInit(), and strictly manage arrays with ArraySetAsSeries(..., false) when forward-indexing is required.
