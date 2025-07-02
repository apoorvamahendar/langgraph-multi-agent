# langgraph-multi-agent

# 🧠 LangGraph Multi-Agent AI – Math Solver & Verifier

This project demonstrates a simple **Agentic AI workflow** using [LangGraph](https://github.com/langchain-ai/langgraph), where multiple agents collaborate to solve and verify a math problem.

---

## 🚀 Project Overview

- **Solver Agent**: Receives a math expression (e.g. `"12 * (5 + 3)"`) and evaluates it.
- **Verifier Agent**: Validates the solution by re-evaluating the original question.
- **LangGraph**: Connects these agents in a defined flow using a state graph.

---

## 📂 Folder Structure

```
langgraph_multi_agent_project_updated/
│
├── agents/
│   ├── solver_agent.py       # Solves math expressions
│   └── verifier_agent.py     # Verifies the computed solution
│
├── main.py                   # Runs the LangGraph workflow
├── requirements.txt          # Python dependencies
├── .env                      # OpenAI API Key (not committed to Git)
└── README.md                 # Project description
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/langgraph-multi-agent-demo.git
cd langgraph-multi-agent-demo
```

### 2. Create and Activate a Virtual Environment

```bash
python -m venv venv
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up `.env`

Create a `.env` file in the root directory:

```
OPENAI_API_KEY=your-openai-api-key
```

---

## ▶️ Run the Application

```bash
python main.py
```

You should see output like:

```
SolverAgent received: 12 * (5 + 3)
Final Output:
{'question': '12 * (5 + 3)', 'solution': 96, 'verified': True, 'message': '✅ Answer verified as correct.'}
```

---

## 🧠 How It Works

This project uses LangGraph to define a **multi-step AI pipeline**:

```
[Solver] → [Verifier] → [END]
```

Each agent modifies a shared `AgentState` dictionary, ensuring data is passed cleanly between steps.

---

## 📌 Requirements

- Python 3.8+
- [LangGraph](https://github.com/langchain-ai/langgraph)
- OpenAI account + API key

---

## 💡 Suggested GitHub Repository Names

You can name your GitHub repository any of the following:

| 🔢 | Suggested Repo Name                     | Description |
|----|-----------------------------------------|-------------|
| 1  | `langgraph-multi-agent-demo`           | General and accurate |
| 2  | `multi-agent-math-graph`               | Highlights the math + LangGraph part |
| 3  | `agentic-ai-langgraph`                 | Emphasizes agentic AI concept |
| 4  | `math-solver-verifier-graph`           | Very specific |
| 5  | `ai-agent-workflow-langgraph`          | SEO optimized |
| 6  | `langgraph-math-bot`                   | Fun and focused |

**Recommended**: `langgraph-multi-agent-demo`

---

## 🛠 Future Improvements

- 🔄 Add GPT-based agents (explanations, question rewriting, etc.)
- 🖥 Streamlit web UI
- 🔒 Error handling and validation
- 📈 Logging & tracing

---

## 📃 License

This project is for educational/demo purposes. You may adapt or extend it under the terms of an MIT-style license.


