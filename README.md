# ✈️ Personalized AI Travel Planner

An AI-powered travel planning assistant built using **Python, LangChain, and LangGraph**. This project explores how LLMs, prompt chaining, AI agents, web search, and conversational memory can work together to generate and refine personalized travel itineraries.

## 🌍 Overview

The **Personalized AI Travel Planner** is a mini project developed to explore the practical applications of Generative AI and agentic workflows.

It combines language models with external search tools and memory to help users plan trips based on their destinations and preferences.

The project also explores LangGraph checkpointing to maintain agent state during conversational interactions.

## ✨ Features

- ✈️ **Personalized Travel Planning:** Generate travel itineraries based on user requests and preferences.
- 🔗 **Prompt Chaining:** Connect prompts and LLMs to process requests through multiple steps.
- ⚙️ **Sequential Processing:** Use connected LLM operations to structure itinerary generation.
- 🤖 **AI Agent:** Use an agent that can decide when to call external search tools.
- 🔎 **Google Search Integration:** Retrieve travel-related information using SerpAPI.
- 🧠 **Conversational Memory:** Use `ConversationBufferWindowMemory` to retain recent conversation context.
- 🔄 **LangGraph Checkpointing:** Explore state management and checkpoint-based memory using `InMemorySaver`.
- 🌐 **OpenRouter Integration:** Connect to language models through the OpenRouter API.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| LangChain | Prompt templates, LLM integration, and chaining |
| LangGraph | Agent workflows and checkpointing |
| OpenRouter | LLM API integration |
| Nemotron | Language model used through OpenRouter |
| SerpAPI | External search integration |
| ConversationBufferWindowMemory | Recent conversational memory |
| InMemorySaver | In-memory checkpointing for LangGraph |

## 🏗️ Workflow

The project explores the following workflow:

1. **User Input:** Receive a destination and travel-related preferences.
2. **Prompt Processing:** Structure the request using LangChain prompt templates.
3. **LLM Chaining:** Process the request through connected language-model operations.
4. **Agent-Based Research:** Allow the agent to use external search tools when needed.
5. **Conversational Memory:** Retain recent conversation context for follow-up requests.
6. **LangGraph Checkpointing:** Save agent state during workflow execution using an in-memory checkpointer.
7. **Itinerary Refinement:** Use conversational interactions to refine travel recommendations.

## 📂 Project Structure

```text
personalized-ai-travel-planner/
│
├── proj.ipynb       # Main project notebook
├── README.md        # Project documentation
├── requirements.txt # Project dependencies
├── .gitignore       # Excludes sensitive and unnecessary files
└── .env.example     # Example environment variable configuration
```

The notebook uses separate Python files for API key configuration. These files should remain private and must not be uploaded to GitHub.

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/personalized-ai-travel-planner.git
cd personalized-ai-travel-planner
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API Keys

Create a `.env` file in the project directory and configure the API keys required by your implementation.

```env
OPENROUTER_API_KEY=your_openrouter_api_key
SERPAPI_API_KEY=your_serpapi_api_key
```

Install `python-dotenv` if your code uses it to load environment variables. Update the notebook's API key imports to read these variables before running it.

**Never upload your actual API keys or private configuration files.**

### 5. Run the Notebook

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `proj.ipynb` and execute the cells in order after configuring your API keys.

## 🧠 Key Concepts Explored

- **Prompt Engineering:** Structuring prompts to guide LLM responses.
- **LangChain Expression Language:** Connecting language-model components into workflows.
- **Sequential Chains:** Passing outputs between multiple LLM operations.
- **Tool Calling:** Connecting agents to external search capabilities.
- **Agentic AI:** Exploring how agents use tools to complete tasks.
- **Conversational Memory:** Maintaining recent chat context across interactions.
- **LangGraph State Management:** Exploring checkpointing and stateful agent workflows.

## 🚀 Future Improvements

- 🌦️ Integrate live weather information.
- 🏨 Add hotel and accommodation recommendations.
- 💰 Include estimated travel budgets.
- 📍 Integrate maps and location-based recommendations.
- 🖥️ Develop a dedicated web interface.
- 💾 Add persistent checkpoint storage.
- 📅 Support more detailed day-by-day itinerary customization.

## 🎯 Learning Outcomes

This project helped me explore how to combine multiple LangChain components into a practical AI application.

It also provided hands-on experience with external tool integration, conversational memory, and LangGraph checkpointing.

As a learning project, it represents an important step in my journey toward **AI Engineering and Agentic AI development**.

## 👨‍💻 Author

**Shreshth Verma**

Aspiring AI Engineer | Exploring Generative AI, LangChain, LangGraph, and Agentic AI.

---

⭐ If you find this project interesting, feel free to explore the repository and share your feedback.

**Built with curiosity and a passion for AI.**
