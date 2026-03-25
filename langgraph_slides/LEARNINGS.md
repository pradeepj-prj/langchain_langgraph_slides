# Learnings — LangGraph Beamer Slides Project

## Library Insights

- LangGraph v1.0 is the first stable release, after widespread adoption by companies like Uber, LinkedIn, and Klarna.
- LangGraph is the low-level orchestration layer underneath LangChain agents. LangChain's create_react_agent is built on LangGraph.
- Core primitives: StateGraph (graph definition), State (shared data with reducers), Nodes (functions), Edges (transitions).
- Checkpointing is built-in and enables persistence, time travel, human-in-the-loop, and crash recovery.
- The `langgraph.prebuilt` module has been deprecated in v1.0; prebuilt agents moved to `langchain.agents`.
- Multi-agent patterns (supervisor, swarm, hierarchical) are first-class citizens via `langgraph-supervisor` and `langgraph-swarm` packages.
- LangGraph Platform provides hosted deployment with built-in persistence, streaming, and monitoring.
- The functional API and Command/Send primitives enable advanced control flow patterns.

## Slide Creation Insights (from LangChain project)

- fontawesome5 package is not available in TeX Live 2022/Debian — do not include.
- Use compact tcolorbox padding (top=2pt, bottom=2pt, left=4pt, right=4pt) from the start to prevent overflow.
- Add aboveskip=2pt, belowskip=2pt to lstset for compact code listings.
- Use [fragile] on all frames with lstlisting; add [shrink=N] for persistently overflowing frames.
- Keep TikZ diagrams to 8-10 nodes max.
- Two-pass pdflatex compilation needed for correct slide numbering.
