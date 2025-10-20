# 🤖 Personal AI Assistant with Gradio & Pushover Integration

[![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)](https://www.python.org/)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-black?logo=openai)](https://platform.openai.com/)
[![Gradio](https://img.shields.io/badge/Gradio-Interface-orange?logo=gradio)](https://gradio.app/)
[![Pushover](https://img.shields.io/badge/Pushover-Notifications-green)](https://pushover.net/)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

An intelligent **AI-powered personal assistant** built with **Gradio** and **OpenAI**, capable of answering questions about myself using data from my LinkedIn profile and a professional summary.  
If the assistant encounters an unknown question or a user shares contact information, it **instantly sends me a Pushover notification**.

---

## ✨ Features

- 💬 **Conversational AI Interface** — Chat with an AI that represents me.
- 📄 **Context-Aware Responses** — Uses my LinkedIn PDF and personal summary to answer questions accurately.
- 🚨 **Pushover Notifications** — Instantly alerts me when:
  - A user shares contact details (email, name, notes).
  - The AI can’t answer a user’s question.
- 🧠 **Function Calling with OpenAI** — Structured tools to record user info or unknown queries.
- 🧩 **Gradio Web UI** — Simple and interactive chat interface.

---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/personal-ai-assistant.git
cd personal-ai-assistant
```

### 2. Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate      # For Linux/Mac
venv\Scripts\activate       # For Windows
```

### 3. Install dependencies
Make sure you have a **`requirements.txt`** file in the root directory, then run:

```bash
pip install -r requirements.txt
```

---

## 🧩 File Structure

```
├── .gitignore
├── .python-version
├── README.md
├── app.ipynb         # Main Program file
├── main.py
├── pyproject.toml
├── requirements.txt
└── uv.lock
```

---

## 🚀 Running the App

```bash
python main.py
```

Then open the local Gradio link in your browser to start chatting with your AI assistant.

---

## 🧠 How It Works

1. Loads your **LinkedIn PDF** and **summary text** into memory.
2. Provides context to OpenAI via a detailed system prompt.
3. Uses **function calling** to:
   - `record_user_details(email, name, notes)` → Sends a Pushover alert when someone shares info.
   - `record_unknown_question(question)` → Sends a Pushover alert for unanswered queries.
4. Runs an interactive **Gradio ChatInterface** frontend.

---

## 🧑‍💻 Author

**Kartik Garg** 

---

> “Your personal AI — always available, always alert.” 🚀
