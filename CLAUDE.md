# LangChain Beamer Slides Project

## Overview
Comprehensive Beamer LaTeX slide deck for learning LangChain v1.2.x (Python). Designed as a complete curriculum from zero knowledge to production proficiency.

## Library Version
- **LangChain**: v1.2.12 (March 2026)
- **LangChain-Core**: v1.2.19
- **Python**: >= 3.10, < 4.0

## Directory Structure

```
langchain_slides/
├── CLAUDE.md                              # This file
├── LEARNINGS.md                           # Lessons learned
├── 00_Overview_and_Architecture/          # Why LangChain, ecosystem map
├── 01_Chat_Models_and_Prompt_Templates/   # Core model interaction
├── 02_Output_Parsing_and_Structured_Output/ # Parsing LLM output
├── 03_Runnables_and_LCEL/                 # Composition & Expression Language
├── 04_Tools_and_Tool_Calling/             # Tool definitions & binding
├── 05_Agents/                             # ReAct agents, reasoning
├── 06_Memory_and_Conversation_Management/ # Chat history & state
├── 07_Document_Loading_and_Text_Splitting/# Ingestion pipeline
├── 08_Embeddings_Vector_Stores_and_Retrievers/ # Similarity search
├── 09_Retrieval_Augmented_Generation/     # End-to-end RAG
├── 10_Callbacks_Streaming_and_Tracing/    # Observability
├── 11_LangGraph_Fundamentals/             # Graph orchestration
├── 12_Deep_Agents_and_Advanced_Orchestration/ # Multi-agent systems
├── 13_Putting_It_All_Together/            # Integrative project
├── 14_Production_and_Best_Practices/      # Deployment patterns
└── 99_Quick_Reference/                    # Cheat sheets
```

## Slide Style
- Beamer with `\usetheme{default}`, no navigation symbols
- Colored tcolorbox highlights: yellow (concepts), red (pitfalls), green (best practices), blue (code)
- Font: Latin Modern (lmodern)
- Slide numbers: N/total format
- TikZ diagrams for architecture, no images

## Section Summary (Final)

| Section | Title | Actual Slides | Study Time |
|---------|-------|---------------|------------|
| 00 | Overview & Architecture | 20 | 30 min |
| 01 | Chat Models & Prompt Templates | 45 | 1.5 hr |
| 02 | Output Parsing & Structured Output | 30 | 1 hr |
| 03 | Runnables & LCEL | 37 | 1.5 hr |
| 04 | Tools & Tool Calling | 40 | 1.5 hr |
| 05 | Agents | 35 | 1.5 hr |
| 06 | Memory & Conversation Management | 37 | 1 hr |
| 07 | Document Loading & Text Splitting | 41 | 1 hr |
| 08 | Embeddings, Vector Stores & Retrievers | 38 | 1.5 hr |
| 09 | Retrieval-Augmented Generation | 36 | 1.5 hr |
| 10 | Callbacks, Streaming & Tracing | 26 | 1 hr |
| 11 | LangGraph Fundamentals | 45 | 2 hr |
| 12 | Deep Agents & Advanced Orchestration | 45 | 2 hr |
| 13 | Putting It All Together | 43 | 2 hr |
| 14 | Production & Best Practices | 41 | 1.5 hr |
| 99 | Quick Reference | 15 | — |
| **Total** | | **574** | **~21 hr** |

## Build Instructions
Each `.tex` file compiles independently:
```bash
cd <section_folder>
pdflatex <filename>.tex
pdflatex <filename>.tex   # second pass for slide numbers
```
