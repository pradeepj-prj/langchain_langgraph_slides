# LangGraph Beamer Slides Project

## Overview
Comprehensive Beamer LaTeX slide deck for learning LangGraph v1.0.x (Python). Designed as a complete curriculum from zero knowledge to production proficiency.

## Library Version
- **LangGraph**: v1.0.x (March 2026)
- **LangChain**: v1.2.x (companion library)
- **Python**: >= 3.10, < 4.0

## Directory Structure

```
langgraph_slides/
├── CLAUDE.md                              # This file
├── LEARNINGS.md                           # Lessons learned
├── 00_Overview_and_Why_LangGraph/         # Motivation, ecosystem, installation
├── 01_State_Nodes_and_Edges/              # Core primitives
├── 02_Building_Your_First_Graph/          # Hands-on graph construction
├── 03_Conditional_Routing_and_Branching/  # Dynamic routing & cycles
├── 04_Tool_Integration/                   # ToolNode, tool calling in graphs
├── 05_Prebuilt_ReAct_Agent/               # create_react_agent shortcut
├── 06_Persistence_and_Checkpointing/      # State saving & threads
├── 07_Human_in_the_Loop/                  # Breakpoints & approval flows
├── 08_Streaming/                          # Stream modes & token streaming
├── 09_Memory/                             # Short-term & long-term memory
├── 10_Subgraphs_and_Modularity/           # Nested graphs & composition
├── 11_Multi_Agent_Patterns/               # Supervisor, swarm, hierarchical
├── 12_Error_Handling_and_Resilience/       # Retries, fallbacks, durability
├── 13_Putting_It_All_Together/            # Integrative project
├── 14_Production_and_LangGraph_Platform/  # Deployment & monitoring
└── 99_Quick_Reference/                    # Cheat sheets
```

## Slide Style
- Beamer with `\usetheme{default}`, no navigation symbols
- Colored tcolorbox highlights: yellow (concepts), red (pitfalls), green (best practices), blue (code)
- Font: Latin Modern (lmodern)
- Slide numbers: N/total format
- TikZ diagrams for architecture, no images
- Compact tcolorbox padding (top=2pt, bottom=2pt) to prevent overflow

## Section Summary (Final)

| Section | Title | Actual Slides | Study Time |
|---------|-------|---------------|------------|
| 00 | Overview & Why LangGraph | 16 | 30 min |
| 01 | State, Nodes & Edges | 24 | 1 hr |
| 02 | Building Your First Graph | 21 | 1 hr |
| 03 | Conditional Routing & Branching | 20 | 45 min |
| 04 | Tool Integration | 20 | 45 min |
| 05 | Prebuilt ReAct Agent | 17 | 30 min |
| 06 | Persistence & Checkpointing | 18 | 45 min |
| 07 | Human-in-the-Loop | 21 | 1 hr |
| 08 | Streaming | 18 | 45 min |
| 09 | Memory | 18 | 45 min |
| 10 | Subgraphs & Modularity | 18 | 45 min |
| 11 | Multi-Agent Patterns | 20 | 1 hr |
| 12 | Error Handling & Resilience | 23 | 1 hr |
| 13 | Putting It All Together | 21 | 1 hr |
| 14 | Production & LangGraph Platform | 22 | 1 hr |
| 99 | Quick Reference | 17 | — |
| **Total** | | **314** | **~13 hr** |

## Build Instructions
Each `.tex` file compiles independently:
```bash
cd <section_folder>
pdflatex <filename>.tex
pdflatex <filename>.tex   # second pass for slide numbers
```
