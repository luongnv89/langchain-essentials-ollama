# 🔗 LangChain Essentails V1.0

## 🚀 Quickstart 

### Prerequisites

Ensure you're have Deno installed:

```bash
# Install Deno
curl -fsSL https://deno.land/install.sh | sh
# Install Deno Jupyter Kernel
deno jupyter --install
# Activate Deno Jupyter Kernel
deno jupyter --unstable
```

You should be able to select the Deno kernel from the available kernels list.

### Installation

1. Clone the repository:
```bash
git clone https://github.com/langchain-ai/lca-langchainV1-essentials.git
cd ./lca-langchainV1-essentials/js
```

2. Install the package and dependencies:
```bash
corepack enable
pnpm install
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

4. Run notebooks with Runme by clicking opening a markdown file in VS Code (or right click on the file and selecting "Open in Runme")