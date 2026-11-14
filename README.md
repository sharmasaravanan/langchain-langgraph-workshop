# Agentic AI Workshop — LangChain & LangGraph

A hands-on workshop covering **Agentic AI fundamentals**, **LangChain**, and **LangGraph** — from first principles to production-ready multi-agent systems.

## 📂 Repository Structure

| File | Description |
|------|-------------|
| `Langchain_Handson.ipynb` | Hands-on notebook covering LangChain core components, LCEL chains, tools, function calling, and agents |
| `Langgraph_Handson.ipynb` | Hands-on notebook covering LangGraph state graphs, conditional workflows, RAG integration, HITL, and multi-agent systems |
| `Agentic AI, From First Principles.html` | Conceptual guide — evolution of LLMs to agents, agent components, lifecycle, and ecosystem |
| `LangGraph & Multi-Agent Systems Workshop.html` | Workshop guide — graph-based workflows, multi-agent patterns, and responsible AI governance |

## 🧠 Topics Covered

### Part 1 — Agentic AI Concepts
- Evolution from LLMs to autonomous agents
- AI agents vs. agentic workflows
- Agent components: models, tools, memory, state & planning
- Agent lifecycle and the current ecosystem

### Part 2 — LangChain Hands-On (`Langchain_Handson.ipynb`)
- **Chat Models** — initialization, batch processing, streaming
- **Prompt Templates & Messages** — `ChatPromptTemplate`, `MessagesPlaceholder`, message types
- **LCEL Chains** — building chains with output parsers and conversation history
- **Tools & Function Calling** — custom tools with `@tool`, binding tools to models, manual tool execution
- **Agents** — `create_agent` with structured output and memory (`InMemorySaver`)

### Part 3 — LangGraph Hands-On (`Langgraph_Handson.ipynb`)
- **Graph Fundamentals** — `StateGraph`, nodes, edges, `START`/`END`
- **Agents with Tools** — `create_react_agent` with calculator, time, and search tools
- **State Management** — typed state with `TypedDict`, persistence with `InMemorySaver`
- **Conditional Workflows** — routing between research, calculation, and general paths
- **RAG Integration** — document splitting, FAISS vector store, retrieval-augmented generation graph
- **Human-in-the-Loop (HITL)** — `interrupt`, `Command`, approval/rejection/editing flows
- **Workflow Control** — iterative loops with sufficiency checks
- **Capstone Project** — AI Research Assistant combining classification, RAG, tools, and HITL

### Part 4 — Multi-Agent Systems & Governance
- Single vs. multi-agent architectures
- Supervisor pattern, specialist agents
- Sequential & parallel agent orchestration
- Agent communication and shared state
- Hallucinations, limitations, and responsible AI

## 🛠️ Prerequisites

- **Python** 3.10+
- **OpenAI API Key** (GPT model access)
- [Google Colab](https://colab.research.google.com/) (recommended) or a local Jupyter environment

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/sharmasaravanan/langchain-langgraph-workshop.git
   cd langchain-langgraph-workshop
   ```

2. **Set up your API key**

   Create a `.env` file in the project root:
   ```
   OPENAI_API_KEY=your-api-key-here
   OPENAI_MODEL=gpt-4o
   ```
   > ⚠️ **Never commit your API key.** The `.gitignore` in this repo excludes `.env` files.

3. **Install dependencies**
   ```bash
   pip install langchain langchain_openai langgraph langchain-community faiss-cpu python-dotenv pydantic
   ```

4. **Open the notebooks**
   - Upload to [Google Colab](https://colab.research.google.com/), or
   - Run locally:
     ```bash
     jupyter notebook
     ```

## 📦 Key Dependencies

| Package | Purpose |
|---------|---------|
| `langchain` | Core framework for chains, agents, and tools |
| `langchain_openai` | OpenAI chat model integration |
| `langgraph` | Graph-based stateful agent workflows |
| `faiss-cpu` | Vector similarity search for RAG |
| `python-dotenv` | Environment variable management |
| `pydantic` | Structured output schemas |

## 📄 License

This project is for educational and workshop purposes.
