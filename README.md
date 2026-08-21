Rufus Agent 🛒

Rufus Agent is an AI-powered shopping assistant inspired by Amazon
Rufus. The project applies concepts from Generative AI and Agentic
AI to create an assistant that can understand a user's shopping
requirements, retrieve relevant information, and help with
product-related decisions.

The project was built to apply practical concepts such as:

-Large Language Models (LLMs)

-LangChain

-Retrieval-Augmented Generation (RAG)

-Vector databases

-AI Agents

-ReAct-style agent workflows

-Product/review information retrieval

-Multimodal AI concepts

-AI evaluation

-Guardrails

✨ What the Project Does

Rufus Agent acts as an intelligent shopping assistant rather than a
simple keyword-based search system.

A user can interact with the assistant using natural language, for
example:

"I need wireless headphones under ₹5,000 with good battery life and
positive reviews."

The agent can use the available information and tools to understand the
request and provide a useful shopping-oriented response.

The project also includes functionality for working with product/review
data and uses an AI agent workflow to process user queries.

📸 Project Demo

Here are some screenshots of Rufus Agent in action.

Add your screenshots to the images folder in the project root and update the filenames below if needed.

🏠 Shopping Assistant



🔎 Product Search & Recommendations



🤖 AI Agent Response



🏗️ Project Structure

tutorial-agentic-ai/
│
├── shopping_agent/
│   ├── app.py              # Streamlit application / user interface
│   ├── shopping_agent.py   # Core AI shopping-agent logic
│   └── reviews_api.py      # Review/product-related API functionality
│
├── main.py                 # Main project entry point / experiments
├── pyproject.toml          # Project dependencies and configuration
├── uv.lock                 # Locked dependency versions
├── .python-version         # Python version used by the project
├── .gitignore              # Files excluded from Git
└── README.md               # Project documentation

Note: Keep your .env file private. It should never be committed
to GitHub because it can contain API keys and other secrets.

🛠️ Tech Stack

Python

LangChain

Google Gemini APIs

Groq APIs

LangSmith for tracing and observability

LLMs / Generative AI

ChromaDB for vector storage

Sentence Transformers for embeddings

Pandas

Streamlit

uv for Python project and dependency management

📋 Prerequisites

Before running the project locally, make sure you have:

Python installed

Git installed

uv installed

Required API keys configured in a .env file

Install uv

If you do not already have uv, install it using the official
installation method for your operating system.

You can verify the installation with:

uv --version

🚀 Installation

1. Clone the repository

git clone <YOUR_GITHUB_REPOSITORY_URL>

Move into the project directory:

cd tutorial-agentic-ai

2. Create the virtual environment and install dependencies

Since this project contains a pyproject.toml and uv.lock, you can
use uv to install the project dependencies:

uv sync

This will create/use the project's virtual environment and install the
dependencies defined in pyproject.toml.

3. Activate the virtual environment

On Windows PowerShell:

.venv\Scripts\Activate.ps1

On Windows Command Prompt:

.venv\Scripts\activate

4. Configure environment variables

Create a .env file inside the directory where the application expects
it.

Example:

GOOGLE_API_KEY=your_api_key_here

If your implementation uses additional APIs, add their keys in the same
.env file.

Never upload real API keys to GitHub.

▶️ Run the Application

Navigate to the application directory:

cd shopping_agent

Start the Streamlit application:

streamlit run app.py

You should see something similar to:

You can now view your Streamlit app in your browser.

Local URL: http://localhost:8501

Open the displayed local URL in your browser.

🧠 How It Works

At a high level, the application follows an agentic workflow:

User Query
    ↓
AI Shopping Agent
    ↓
Understand User Intent
    ↓
Reason / Decide What Information Is Needed
    ↓
Use Available Tools / Retrieval
    ↓
Process Product & Review Information
    ↓
Generate Response
    ↓
Shopping Recommendation / Assistance

The important difference from a traditional application is that the LLM
is used as part of an agentic workflow, allowing the system to
reason about the request and determine how to use the available
information/tools.

🔐 Environment Variables

The .env file is intentionally excluded from version control.

Make sure your .gitignore contains:

.env

If an API key has already been pushed to a public repository,
revoke/rotate that key immediately and then remove the secret from
the repository history.

🧪 Running the Project

Typical local workflow:

# Clone
git clone <YOUR_GITHUB_REPOSITORY_URL>

# Enter project
cd tutorial-agentic-ai

# Install dependencies
uv sync

# Activate environment
.venv\Scripts\Activate.ps1

# Enter application directory
cd shopping_agent

# Run Streamlit
streamlit run app.py

🎯 Learning Outcomes

This project was created as a practical application of Agentic AI
concepts learned during my Agentic AI certification.

Through this project, I worked with concepts including:

Generative AI and LLM fundamentals

RAG and vector databases

AI agents

ReAct loops

Tool-based agent workflows

Multi-agent concepts

Multimodal AI

Evaluation

Guardrails

The main goal was to move from learning AI concepts to actually
implementing them in a working application.

🚧 Future Improvements

-Possible future improvements include:

-Product comparison across multiple sources

-Better recommendation ranking

-Conversation memory

-More shopping tools

-Improved agent evaluation

-Stronger guardrails

-Multi-agent shopping workflows

-Better UI/UX

-Deployment to a cloud platform

👨‍💻 Author

Ansh Verma

Built as a hands-on project while learning and exploring Generative AI
and Agentic AI.
