AI_Agent


Welcome to AI_Agent — a flexible and modular agent framework built for intelligent task execution using Large Language Models (LLMs).
This project combines powerful reasoning abilities with tool integrations, enabling the agent to solve complex problems autonomously.

🚀 Features
LLM-driven Agent:
Core agent uses OpenAI's GPT models for reasoning and action planning.

Tool Abstraction:
Plug-and-play design to easily add custom tools or APIs for the agent to use during its reasoning steps.

ReAct-based Reasoning:
Implements the ReAct (Reasoning + Acting) pattern for structured thought, action selection, and final answer generation.

Extensible and Lightweight:
Easily customizable agent architecture for different use cases like web search, calculations, data analysis, and more.

🛠 Project Structure

AI_Agent/
├── agents/
│   ├── base_agent.py       # Core agent logic (ReAct-style reasoning and action loop)
│   └── agent_with_memory.py # (Work in progress) Agent variant with memory
│
├── tools/
│   ├── base_tool.py         # Tool interface blueprint
│   ├── web_search_tool.py   # Example tool: Search the web
│   └── calculator_tool.py   # Example tool: Perform basic math
│
├── prompts/
│   └── react_prompt.txt     # Prompt template for ReAct reasoning
│
├── configs/
│   └── config.yaml          # API keys, model configurations, tool lists
│
├── main.py                  # Sample runner file to initialize and run the agent
└── requirements.txt         # Python dependencies

🧠 How It Works
The agent operates in a thought-action-observation loop:

Think about the task.

Select a tool and act.

Observe the result.

Repeat until the final answer is generated.

It uses a prompt-based framework where the LLM reasons about which tool to use and how to proceed step-by-step.

📦 Setup Instructions
Clone the repository:

git clone https://github.com/haashu0412/Ai_Agent.git
cd Ai_Agent

Install dependencies:

pip install -r requirements.txt

Set up your API keys:
Open configs/config.yaml

Run the agent:

python main.py

📋 Requirements
Python 3.8+

OpenAI API key (for LLM-based reasoning)

Internet access (for tools like web search)

📚 Future Work
Add memory integration (agent_with_memory.py)

Introduce multi-agent collaboration

Expand toolset: database querying, API interaction, file system access

Improve error handling and agent introspection

🤝 Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request.
For major changes, please open an issue first to discuss what you would like to change.

