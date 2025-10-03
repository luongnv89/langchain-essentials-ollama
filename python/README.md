# 🔗 LangChain Essentails V1.0



## 🚀 Quickstart 

### Prerequisites

- Ensure you're using Python 3.11 or later.
- This version is required for optimal compatibility with LangGraph.
```bash
python3 --version
```
- [uv](https://docs.astral.sh/uv/) package manager
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
# Update PATH to use the new uv version
export PATH="/Users/$USER/.local/bin:$PATH"
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/langchain-ai/lca-langchainV1-essentials.git
```

1. cd python

3. Install the package and dependencies (this automatically creates and manages the virtual environment):
```bash
uv sync
```

3. Create a `.env` file in the project root with your API keys:
```bash
# Create .env file
cp example.env .env
```

Add your API keys to the `.env` file:
```env

# Required for model usage
OPENAI_API_KEY=your_openai_api_key_here

# Optional: For evaluation and tracing
LANGSMITH_API_KEY=your_langsmith_api_key_here
LANGSMITH_TRACING=true
LANGSMITH_PROJECT=lc-essentials
```

4. Run notebooks or code using uv:
```bash
# Run Jupyter notebooks directly
uv run jupyter notebook

# Or activate the virtual environment if preferred
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
jupyter lab
```

## 📚 Tutorial Overview

This repository contains two notebooks. The first covers the foundations of LangGraph that will enable you to build any workflow or AI agent. In the second, you will build an example LangGraph workflow.

### `L1.ipynb` - StateGraph Essentials
- You will use all the components of LangGraph
    - State and Nodes
    - Edges
        - Parallel
        - Conditional
    - Memory
    - Interrupts/ Human-In-The-Loop  

### `L2.ipynb` - Build A Workflow
Learn to implement structured workflow to process customer emails. This notebook utilizes all of the building blocks from the first notebook in an example application.:
- Task tracking with status management (pending/in_progress/completed)  

