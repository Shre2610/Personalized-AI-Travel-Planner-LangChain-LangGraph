# ✈️ Personalized AI Travel Planner

An AI-powered travel planning assistant built with **LangChain, LangGraph, and Python**. It generates personalized travel itineraries based on user preferences and supports conversational refinement using AI agents, external search, and memory.

## 🌍 Overview

Planning a trip often involves researching destinations, exploring attractions, and organizing activities around personal preferences.

The **Personalized AI Travel Planner** aims to simplify this process using Large Language Models (LLMs), prompt chaining, and AI agents.

Users can provide a destination and travel preferences to generate an itinerary, explore attractions through search, and refine their travel plans through conversation.

This project was developed as a hands-on learning experience to explore the LangChain ecosystem and agentic AI workflows.

## ✨ Features

- 🗺️ **Personalized Itinerary Generation**  
  Generate travel itineraries based on the destination and user preferences.

- 🔗 **LLM & Prompt Chaining**  
  Connect prompts and language models to process travel requests through multiple steps.

- ⚙️ **Sequential Processing**  
  Use sequential chains to organize itinerary generation into connected LLM operations.

- 🤖 **AI Agent Integration**  
  Use an AI agent to decide when to call external tools for travel research.

- 🔎 **Google Search Integration**  
  Search for tourist attractions and destination-related information.

- 🧠 **Conversational Memory**  
  Retain relevant conversation context and user preferences for more personalized interactions.

- 🔄 **LangGraph Checkpointing**  
  Explore checkpoint-based memory and conversational workflows for maintaining agent state.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| LangChain | LLM integration, prompt templates, and chaining |
| LangGraph | Agent workflows and checkpoint-based state management |
| Large Language Models | Itinerary generation and conversational responses |
| SerpAPI | Google Search integration |
| Python Environment Variables | Secure API key configuration |

## 🏗️ How It Works

The application follows a conversational travel-planning workflow:

1. **User Input:** The user provides a destination and travel preferences.
2. **Prompt Processing:** Prompt templates structure the request for the language model.
3. **Sequential Chain Execution:** Connected LLM operations help generate the itinerary.
4. **Agent-Based Research:** The AI agent can use search tools to retrieve relevant travel information.
5. **Memory and Context:** Conversation history and checkpointing help preserve relevant context.
6. **Itinerary Refinement:** The user can ask follow-up questions and refine the generated travel plan.

## 📂 Project Structure

```text
personalized-ai-travel-planner/
│
├── main.py                 # Main application entry point
├── requirements.txt        # Project dependencies
├── .env                    # API keys (not committed)
├── .gitignore              # Files excluded from Git
├── README.md               # Project documentation
│
└── notebooks/              # Optional experiments and learning notebooks
```

*Note: Update this structure to match the actual files in your repository.*

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

Activate it:

**Windows**
```bash
venv\Scripts\activate
```

**macOS / Linux**
```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API Keys

Create a `.env` file in the project root and add the API keys required by your configuration.

```env
GOOGLE_API_KEY=your_google_api_key
SERPAPI_API_KEY=your_serpapi_api_key
```

Use the environment variables that match your actual model and search integrations. Never commit your real API keys to GitHub.

### 5. Run the Project

If your application entry point is `main.py`, run:

```bash
python main.py
```

Follow the instructions displayed by your application.

## 🔐 Environment Variables

| Variable | Description |
|---|---|
| `GOOGLE_API_KEY` | API key for Google AI models, if used |
| `SERPAPI_API_KEY` | API key for SerpAPI search integration |

Only configure the keys needed by your implementation.

## 📚 Key Concepts Explored

This project provided practical experience with:

- **Prompt Engineering:** Designing structured prompts for more useful LLM responses.
- **LCEL and Chaining:** Connecting prompts, models, and output processing.
- **Sequential Chains:** Passing outputs between multiple LLM operations.
- **Tool Calling:** Allowing an agent to use external search capabilities.
- **Agentic Workflows:** Exploring how agents select tools and respond to user requests.
- **Conversational Memory:** Maintaining context across multiple interactions.
- **LangGraph Checkpointing:** Exploring state persistence in agent workflows.

## 🚀 Future Improvements

Some ideas for extending the project:

- 🌦️ Integrate live weather information for travel destinations.
- 🏨 Add hotel and accommodation recommendations.
- 💰 Include estimated travel budgets and expense breakdowns.
- 📍 Integrate maps and location-based recommendations.
- 🖥️ Build a polished web interface.
- 💾 Improve persistent memory and support multiple user sessions.
- 📅 Add travel duration and day-by-day itinerary customization.

## 🎯 Learning Outcome

Building this project helped me understand how individual LangChain components can work together to create a more capable AI application.

It also gave me an opportunity to explore how **LangGraph can support stateful agent workflows** through checkpointing.

This is a learning project and an ongoing step in my journey toward **AI Engineering**.

## 👨‍💻 Author

**Shreshth Verma**

Aspiring AI Engineer | Exploring Generative AI, LangChain, LangGraph, and Agentic AI.

---

⭐ If you find this project interesting, feel free to explore the repository and share your feedback.

**Built with curiosity and a passion for AI.**
