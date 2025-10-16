# 🔗 LangChain Essentials Python


## 🚀 Setup 

### Prerequisites

- Ensure you're using Python 3.11 - 3.13.
- [uv](https://docs.astral.sh/uv/) package manager or [pip](https://pypi.org/project/pip/)
- OpenAI API key

### Installation

```bash
# Clone the repo, cd to 'python' directory
git clone https://github.com/langchain-ai/lca-langchainV1-essentials.git
cd ./lca-langchainV1-essentials/python

# Create .env file
cp example.env .env

# Add OpenAI API key
OPENAI_API_KEY=your_openai_api_key_here

# Create environment
uv sync

# Run Jupyter notebooks directly with uv
uv run jupyter lab

# Or activate the virtual environment if preferred
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
jupyter lab
```

Setup [LangSmith Studio](https://docs.langchain.com/oss/python/langchain/studio)

```bash
# copy the .env file you created above to the studio directory
cp .env ./studio/.

#to run
langgraph dev
```

**Optional:** LangSmith for evaluation and tracing

- Create a [LangSmith](https://smith.langchain.com/) account
- Create a LangSmith API key
<img width="1196" height="693" alt="Screenshot 2025-10-16 at 8 28 03 AM" src="https://github.com/user-attachments/assets/e39b8364-c3e3-4c75-a287-d9d4685caad5" />
<img width="1196" height="468" alt="Screenshot 2025-10-16 at 8 29 57 AM" src="https://github.com/user-attachments/assets/2e916b2d-e3b0-4c59-a178-c5818604b8fe" />


```env
# Add your API key to your .env file
LANGSMITH_API_KEY=your_langsmith_api_key_here
LANGSMITH_TRACING=true
LANGSMITH_PROJECT=lc-essentials
```

# Lessons
This repository contains nine short notebooks that serve as brief introductions to many of the most-used features in LangChain, starting with the new **Create Agent**.

---

### `L1_fast_agent.ipynb` - 🤖 Create Agent 🤖
- In this notebook, you will use LangChain’s `create_agent` to build an SQL agent in just a few lines of code.  
- It demonstrates how quick and easy it is to build a powerful agent. You can easily take this agent and apply it to your own project. 
- You will also use **LangSmith Studio**, a handy visual debugger to run, host, and explore agents.

---

### `L2-7.ipynb` - 🧱 Building Blocks 🧱
In Lessons 2–7, you will learn how to use some of the fundamental building blocks in LangChain. These lessons explain and complement `create_agent`, and you’ll find them useful when creating your own agents. Each lesson is concise and focused.

- **L2_messages.ipynb**: Learn how messages convey information between agent components.  
- **L3_streaming.ipynb**: Learn how to reduce user-perceived latency using streaming.  
- **L4_tools.ipynb**: Learn basic tool use to enhance your model with custom or prebuilt tools.  
- **L5_tools_with_mcp.ipynb**: Learn to use the LangChain MCP adapter to access the world of MCP tools.  
- **L6_memory.ipynb**: Learn how to give your agent the ability to maintain state between invocations.  
- **L7_structuredOutput.ipynb**: Learn how to produce structured output from your agent.  

---

### `L8-9.ipynb` - 🪛 Customize Your Agent 🤖
Lessons 2–7 covered out-of-the-box features. However, `create_agent` also supports both prebuilt and user-defined customization through **Middleware**. This section describes middleware and includes two lessons highlighting specific use cases.

- **L8_dynamic.ipynb**: Learn how to dynamically modify the agent’s system prompt to react to changing contexts.  
- **L9_HITL.ipynb**: Learn how to use Interrupts to enable Human-in-the-Loop interactions.





## 📚 Tutorial Overview

This repository contains nine short notebooks which are brief introductions many of the most-used features in LangChain starting with the new Create Agent.

### `L1_fast_agent.ipynb` - 🤖 Create Agent 🤖
- In this notebook, you will build and use LangChain's `create_agent` to build an SQL agent in a few lines of code.
- This notebook demonstrates how quick and easy it is to build a very powerful agent.
- You will also use LangSmith Studio, a handy visual debugger to run, host, and explore agents.


### `L2-7.ipynb` - 🧱 Building blocks 🧱
In Lessons 2-7, you will learn to use some of the building blocks in LangChain. These explain and complement `create_agent`, and you will find them useful when creating your own agents. There are many lessons, but each is a quick look.

 - **L2_messages.ipynb**: Learn how messages convey information between components of the agent.
 - **L3_streaming.ipynb**: Learn to reduce user-perceived latency using streaming.
 - **L4_tools.ipyb**: Learn basic tool use to enhance your model with custom or prebuilt tools.
 - **L5_tools_with_mcp.ipynb**: Learn to use the Langchain mcp adaptor to access the world of mcp tools.
 - **L6_memory.ipynb**: Learn to give your agent the ability to maintain state between invocations.
 - **L7_structuredOutput.ipynb**: Learn to use your agent to produce structured output.
 - 
### L8-9.ipynb - 🪛 Customize Your Agent 🤖
Lessons 2-7 covered out-of-the-box features. However, `create_agent` supports pre-built and user-created customization by adding access to the agent via Middleware. This section describes middleware and has two lessons on particular instances of its use.

- **L8_dynamic.ipynb**: Learn to create and change the agents' system prompt on the fly to react to current situations.
- **L9_HITL.ipynb**: Learn to use Interrupts to gain Human in the Loop interactions.

