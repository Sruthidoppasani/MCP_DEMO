# 🤖 MCP Agent with Cursor
An AI-powered agent built using Model Context Protocol (MCP), where the agent can interact with external tools through MCP servers while maintaining conversation memory across interactions.

The project uses Qwen3:8B running locally through Ollama as the language model and MCPAgent from mcp-use to manage the agent workflow.

## 🌟 Project Overview

Traditional LLM applications mainly generate responses based on the information available to the model.

With **MCP**, an AI agent can connect to external tools and services and use them according to the user's request.

In this project:

**User → Qwen3:8B → LLM → MCP Servers → External Tools → Response**


## 🧩 MCP Servers Used

### 🎭 Playwright MCP

Used for browser automation and interacting with web pages.

Examples:

* Open websites
* Navigate through pages
* Search for information
* Interact with web elements

### 🏠 Airbnb MCP

Used for searching accommodation-related information.

Examples:

* Search for stays
* Find available accommodation options
* Retrieve relevant property information

### 🔎 DuckDuckGo Search MCP

Used for web-based information retrieval.

Examples:

* Search the web
* Find recent information
* Retrieve relevant search results

## 🛠️ Tech Stack

* **Python**
* **MCP (Model Context Protocol)**
* **mcp-use**
* **Ollama**
* **Qwen3.8B**
* **Cursor**
* **Playwright**
* **DuckDuckGo Search**
* **Airbnb MCP**

## ✨ Key Features

* 🤖 AI agent powered workflow
* 🔌 MCP-based tool integration
* 🌐 Web search capabilities
* 🎭 Browser automation
* 🏠 Accommodation search
* 🧠 LLM-powered tool selection
* 🔄 Multiple MCP servers working together
* 💬 Natural-language interaction

## 📂 Project Structure

```text
mcp-agent/
│
├── main.py
├── requirements.txt
├── .env
├── README.md
│
└── ...
```

> The exact file structure may vary depending on your implementation.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd mcp-agent
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
```

Add any other API keys required by the MCP servers you configure.

## ▶️ Running the Project

Run the agent using:

```bash
python main.py
```

Once the agent is running, provide a natural-language request.

For example:

```text
Search for the latest AI news and give me two headlines.
```

The agent can determine which MCP tool is appropriate and use it to complete the task.

## 🔄 How It Works

```text
                 ┌─────────────────┐
                 │      User       │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │   Qwen3:8B 
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │       LLM       │
                 └────────┬────────┘
                          │
              ┌───────────┼───────────┐
              ▼           ▼           ▼
        ┌──────────┐ ┌──────────┐ ┌──────────┐
        │Playwright│ │ DuckDuckGo│ │  Airbnb  │
        │   MCP    │ │    MCP    │ │   MCP    │
        └────┬─────┘ └────┬─────┘ └────┬─────┘
             │            │            │
             └────────────┼────────────┘
                          ▼
                 ┌─────────────────┐
                 │  Tool Response  │
                 └────────┬────────┘
                          ▼
                 ┌─────────────────┐
                 │ Agent Response  │
                 └─────────────────┘
```

## 🎯 Example Use Cases

This architecture can be extended to build agents capable of:

* 🔎 Researching information from the web
* 📰 Finding recent news
* 🌐 Automating browser-based tasks
* ✈️ Planning travel
* 🏨 Searching for accommodation
* 📊 Collecting information from multiple sources
* 🔗 Connecting multiple external tools to one AI agent

## 📚 What I Learned

Through this project, I gained practical experience with:

* Model Context Protocol (MCP)
* AI agent architecture
* Tool calling
* LLM integration
* Browser automation
* MCP server configuration
* Multi-tool agent workflows
* Building AI applications with Python

## 🚀 Future Improvements

Some improvements I plan to explore:

* [ ] Add more MCP servers
* [ ] Improve agent planning and reasoning
* [ ] Add persistent conversation memory
* [ ] Add more browser automation workflows
* [ ] Build a web-based user interface
* [ ] Improve error handling
* [ ] Add more real-world agent workflows


## 👩‍💻 Author

**Sruthi Doppasani**

Interested in **Artificial Intelligence, Machine Learning, Generative AI, AI Agents, and MCP-based applications**.

---

⭐ If you find this project interesting, consider giving the repository a star!
