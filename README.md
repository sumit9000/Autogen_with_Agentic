# AutoGen and Agentic AI – Multi-Agent Intelligence with Conversations

![Status](https://img.shields.io/badge/status-active-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Python](https://img.shields.io/badge/python-3.10+-yellow)

---

## 🔹 Short Description

This project explores **AutoGen** and **Agentic AI** — advanced technologies that allow AI agents (like ChatGPT) to work together in conversations to complete complex tasks. Using Python and OpenAI, we simulate how multiple intelligent agents interact, learn, and solve problems—similar to how real people collaborate in teams.

---

## 🧠 What Is AutoGen?

> **AutoGen** is a Python framework created by Microsoft that allows different AI agents to collaborate by talking to each other in a structured way.

### Real-World Analogy:
Imagine you’re organizing a school event:
- One student handles decorations 🎨
- Another prepares the schedule 🕒
- One manages the budget 💰

They chat and coordinate together. **AutoGen does this with AI bots.**

---

## 🤖 What is Agentic AI?

**Agentic AI** is the idea of building AI agents that:
- Can **think and act** independently
- Can **make decisions**
- Can **collaborate** with humans or other agents

### Think of it like:
> A team of robots working together—each with a brain, a purpose, and the ability to talk and decide what to do next.

---

## 💡 Topics Covered (Beginner-Friendly)

| Topic | Explanation |
|-------|-------------|
| **AutoGen** | A tool to create intelligent agents that talk and work together. |
| **Agentic Workflow** | The flow of tasks between agents as they collaborate. |
| **Multi-Agent Conversations** | Agents chatting to share tasks and thoughts. |
| **OpenAI/GPT Integration** | Using ChatGPT-like models to give agents intelligence. |
| **UserProxyAgent** | An agent that mimics user decisions or asks for your input. |
| **AssistantAgent** | An AI worker agent that can perform tasks like writing or coding. |
| **Conversational Programming** | Letting agents talk and solve tasks instead of using traditional logic or scripts. |
| **Task Completion via Dialogue** | Agents work through discussion until the goal is reached. |
| **Python Notebook** | Code written in a beginner-friendly notebook format (Jupyter). |

---

## 🔁 How It Works

1. **Define Agents** – Give each AI bot a name and task (e.g., Writer, Checker)
2. **Set Objective** – Example: "Write a blog post about climate change"
3. **Start the Conversation** – Agents exchange messages and collaborate
4. **Monitor or Intervene** – You can step in and guide if needed
5. **Finish** – The team produces the final result (e.g., a full article)

---

## 📸 Visual Diagrams

### 🧠 Agent Collaboration Flow

name: Run Jupyter Notebook

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  run-notebook:
    runs-on: ubuntu-latest

    steps:
    - name: 📥 Checkout Repository
      uses: actions/checkout@v3

    - name: 🐍 Set Up Python
      uses: actions/setup-python@v4
      with:
        python-version: '3.10'

    - name: 📦 Install Dependencies
      run: |
        python -m pip install --upgrade pip
        pip install -r requirements.txt
        pip install nbconvert jupyter nbformat

    - name: ▶️ Run Jupyter Notebook
      run: |
        jupyter nbconvert --to notebook --execute Autogen_and_agentic.ipynb --output executed_notebook.ipynb


---

## 🧪 Real-Life Example: Writing a Blog Post

### Objective: “Write a blog post on AI in Education”

**Agent Roles:**
- ✍️ `WriterAgent` – Generates the content
- 🕵️ `EditorAgent` – Proofreads and improves writing
- 📢 `PublisherAgent` – Suggests how to share the article online
- 👩‍💻 `UserProxyAgent` – You! You can accept or reject suggestions

They talk, plan, fix each other’s work, and produce a full blog article.

---

## 🛠️ Requirements

- Python 3.10+
- OpenAI API key
- Jupyter Notebook
- AutoGen (`pip install pyautogen`)

---



## 🚀 Run This Project

```bash
git clone https://github.com/yourusername/autoagent-intro.git
cd autoagent-intro
pip install -r requirements.txt
jupyter notebook Autogen_and_agentic.ipynb
