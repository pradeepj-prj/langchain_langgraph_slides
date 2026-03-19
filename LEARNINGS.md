# Learnings — LangChain Beamer Slides Project

## Library Insights

- LangChain v1.2.x (2026) has matured into an "agent engineering platform" — the focus has shifted from chains to agents as the primary abstraction.
- The package is now modular: `langchain-core` for interfaces, `langchain` for high-level features, provider-specific packages (`langchain-openai`, `langchain-anthropic`, etc.) for integrations.
- LangChain Expression Language (LCEL) with the pipe operator is the canonical way to compose components. Legacy `LLMChain` and similar classes are in `langchain-classic`.
- LangGraph is the low-level orchestration layer; LangChain agents are built on top of LangGraph.
- Deep Agents (new in 2026) provide planning, sub-agent spawning, and filesystem-backed context management for long-running tasks.
- MCP (Model Context Protocol) adapters bridge LangChain to the broader MCP ecosystem.

## Slide Creation Insights

- fontawesome5 package is not available in TeX Live 2022/Debian — removed from preamble early on.
- Code-heavy Beamer slides frequently trigger overfull vbox warnings — these are cosmetic and don't affect readability.
- The `[fragile]` frame option is essential for any slide containing lstlisting or verbatim environments.
- tcolorbox with color-coded categories (yellow=concepts, red=warnings, green=tips, blue=code) works very well for technical learning material.
- TikZ diagrams are effective for architecture overviews and data flow visualization, but should be kept to 8-10 nodes max for readability on slides.
- Two-pass pdflatex compilation is needed for correct slide numbering (N/total).
- Targeting 30-50 slides per section with ~1-2 hours of study time per section is a good balance between depth and digestibility.
- Total output: 574 slides across 16 decks, covering ~21 hours of study material.
