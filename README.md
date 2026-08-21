# Rufus Agent 🛒

Rufus Agent is an **AI-powered shopping assistant** inspired by Amazon Rufus. The project applies concepts from **Generative AI and Agentic AI** to create an assistant that can understand a user's shopping requirements, retrieve relevant information, and help with product-related decisions.

The project was built to apply practical concepts such as:

* Large Language Models (LLMs)
* LangChain
* Retrieval-Augmented Generation (RAG)
* Vector Databases
* AI Agents
* ReAct-style agent workflows
* Product and review information retrieval
* Multimodal AI concepts
* AI Evaluation
* Guardrails

## ✨ What the Project Does

Rufus Agent acts as an intelligent shopping assistant rather than a simple keyword-based search system.

A user can interact with the assistant using natural language, for example:

> "I need wireless headphones under ₹5,000 with good battery life and positive reviews."

The agent can understand the user's requirements, process the available product and review information, and provide a useful shopping-oriented response.

The main goal of this project is to demonstrate how **Agentic AI concepts can be applied to build a real-world AI-powered shopping application.**

---

## 📸 Project Demo

Here are some screenshots of Rufus Agent in action.

### 🏠 Shopping Assistant

![Rufus Agent Home](./images/demo-home.png)

### 🔎 Product Search & Recommendations

![Product Recommendations](./images/shopping-result.png)

### 🤖 AI Agent Response

![Agent Response](./images/agent-response.png)

---

## 🏗️ Project Structure

```text
tutorial-agentic-ai/
│
├── shopping_agent/
│   ├── app.py              # Streamlit application / user interface
│   ├── shopping_agent.py   # Core AI shopping-agent logic
│   └── reviews_api.py      # Review/product-related API functionality
│
├── images/
│   ├── demo-home.png
│   ├── shopping-result.png
│   └── agent-response.png
│
├── main.py                 # Main project entry point / experiments
├── pyproject.toml          # Project dependencies and configuration
├── uv.lock                 # Locked dependency versions
├── .python-version         # Python version used by the project
├── .gitignore              # Files excluded from Git
└── README.md               # Project documentation
```

> **Note:** Keep your `.env` file private. It should never be committed to GitHub because it can contain API keys and other secrets.

---

## 🛠️ Tech Stack

* **Python**
* **LangChain**
* **Google Gemini APIs**
* **Groq APIs**
* **LangSmith** for tracing and observability
* **LLMs / Generative AI**
* **ChromaDB** for vector storage
* **Sentence Transformers** for embeddings
* **Pandas**
* **Streamlit**
* **uv** for Python project and dependency management

---

## 📋 Prerequisites

Before running the project locally, make sure you have:

1. Python installed
2. Git installed
3. `uv` installed
4. Required API keys configured in a `.env` file

### Install uv

You can install `uv` using its official installation method.

Verify the installation:

```bash
uv --version
```

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

Move into the project directory:

```bash
cd tutorial-agentic-ai
```

### 2. Install Dependencies

Since this project uses `pyproject.toml` and `uv.lock`, install the dependencies using:

```bash
uv sync
```

This will create/use the project's virtual environment and install the required dependencies.

### 3. Activate the Virtual Environment

On Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

On Windows Command Prompt:

```cmd
.venv\Scripts\activate
```

---

## 🔐 Environment Variables

Create a `.env` file inside the project directory and add the required API keys.

Example:

```env
GOOGLE_API_KEY=your_google_api_key
GROQ_API_KEY=your_groq_api_key
LANGSMITH_API_KEY=your_langsmith_api_key
LANGSMITH_TRACING=true
LANGSMITH_PROJECT=Rufus-Agent
```

Depending on your implementation, you may only need some of these variables.

**Never upload your actual API keys to GitHub.**

Make sure your `.gitignore` contains:

```gitignore
.env
```

If an API key has already been pushed to a public repository, **revoke or rotate the key immediately.**

---

## ▶️ Run the Application

Navigate to the application directory:

```bash
cd shopping_agent
```

Start the Streamlit application:

```bash
streamlit run app.py
```

You should see something similar to:

```text
You can now view your Streamlit app in your browser.

Local URL: http://localhost:8501
```

Open the displayed local URL in your browser.

---

## 🧠 How It Works

At a high level, Rufus Agent follows an agentic workflow:

```text
User Query
    ↓
AI Shopping Agent
    ↓
Understand User Intent
    ↓
Reason About the Request
    ↓
Retrieve Relevant Information
    ↓
Use Available Tools / APIs
    ↓
Process Product & Review Information
    ↓
Generate AI Response
    ↓
Shopping Recommendation / Assistance
```

The application uses an **AI agent workflow** rather than relying only on traditional keyword-based search.

The agent can understand the user's natural-language request and use the available information and tools to generate a relevant response.

---

## 🔄 Agentic AI Concepts Applied

This project was built while learning and experimenting with several important Agentic AI concepts:

### Generative AI & LLMs

Used Large Language Models to understand natural-language queries and generate responses.

### RAG

Retrieval-Augmented Generation allows the application to retrieve relevant information and use it as context while generating responses.

### Vector Database

ChromaDB is used for storing and retrieving vector representations of information.

### AI Agents

The shopping agent can reason about the user's request and determine how to process the query using available tools and information.

### ReAct Workflow

The project explores the **Reason + Act** approach where an agent can reason about a task and perform actions using available tools.

### Evaluation

LangSmith is used for tracing and observing the application's AI workflows and helping evaluate agent behavior.

### Guardrails

Guardrails help make AI applications more reliable and controlled by defining boundaries around the agent's behavior.

---

## 🧪 Example Query

A user can ask:

```text
I am looking for a laptop under ₹70,000
with good battery life and suitable for programming.
```

The agent can then analyze the requirements and provide a shopping-oriented response based on the available product and review information.

---

## 🎯 Learning Outcomes

This project was created as a practical application of concepts learned during my **Agentic AI certification**.

Through this project, I gained hands-on experience with:

* Generative AI and LLM fundamentals
* Transformer and LLM concepts
* RAG
* Vector databases
* AI Agents
* ReAct loops
* Tool-based agent workflows
* Multi-Agent system concepts
* Multimodal AI
* AI evaluation
* Guardrails
* LangChain
* LangSmith
* Google Gemini APIs
* Groq APIs

The main objective was to move from **learning AI concepts to implementing them in a real-world application.**

---

## 🚧 Future Improvements

Possible future improvements include:

* Product comparison across multiple sources
* Better recommendation ranking
* Conversation memory
* More shopping tools
* Improved agent evaluation
* Stronger guardrails
* Multi-agent shopping workflows
* Better UI/UX
* Cloud deployment
* Personalized recommendations

---

## 👨‍💻 Author

**Ansh Verma**

Built as a hands-on project while learning and exploring **Generative AI and Agentic AI**.

**Learning → Applying → Building 🚀**

