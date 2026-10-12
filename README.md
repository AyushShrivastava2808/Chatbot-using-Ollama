# 🤖 Google Gemma Chatbot using Ollama

A lightweight AI chatbot built with **Python, Streamlit, LangChain, and Ollama**, powered by the Google Gemma 3 large language model. The application allows users to enter questions through a simple web interface and receive AI-generated responses from a locally running model.

The project demonstrates how to integrate an open-source LLM with a Python application using LangChain and Ollama.

## ✨ Features

- 🤖 **Google Gemma 3:** Generate responses using the Gemma 3 language model.
- 🖥️ **Interactive Web Interface:** A simple interface built with Streamlit.
- 🔗 **LangChain Integration:** Connect the application to the language model through LangChain.
- 🏠 **Local Model Execution:** Run inference locally using Ollama without requiring a cloud-based LLM API.
- ⚡ **Simple Setup:** Install dependencies and launch the chatbot with a few commands.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Application development |
| Streamlit | Web interface |
| LangChain | LLM integration |
| Ollama | Local model runtime |
| Google Gemma 3 | Language model |
| python-dotenv | Environment variable management |

## 📁 Project Structure

```text
Chatbot-using-Ollama/
│
├── ollama.py
├── requirements.txt
├── .gitignore
└── README.md
```

## ⚙️ Prerequisites

Before running the project, ensure you have:

- Python 3.10 or a compatible version
- Ollama installed on your system
- Git installed
- Sufficient RAM and disk space to run the selected model

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/AyushShrivastava2808/Chatbot-using-Ollama.git
```

Navigate to the project directory:

```bash
cd Chatbot-using-Ollama
```

### 2. Create a virtual environment

**Windows:**

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Download the Gemma 3 model

Ensure Ollama is installed and running. Then execute:

```bash
ollama pull gemma3
```

This downloads the model required by the application. Model storage requirements depend on the selected model variant.

### 5. Run the chatbot

Start the Streamlit application:

```bash
streamlit run ollama.py
```

Open the local URL displayed in your terminal, typically:

```text
http://localhost:8501
```

## 💬 How It Works

The application follows a straightforward workflow:

1. The user enters a question in the Streamlit interface.
2. The application passes the question to the Gemma 3 model through LangChain.
3. Ollama runs the model locally and generates a response.
4. The generated response is displayed in the Streamlit interface.

```text
User Input
    ↓
Streamlit Interface
    ↓
LangChain Integration
    ↓
Ollama Runtime
    ↓
Google Gemma 3
    ↓
Generated Response
    ↓
Streamlit Output
```

## 🧠 Key Learnings

This project provides practical experience with:

- Integrating locally hosted large language models into Python applications.
- Using LangChain to invoke an LLM.
- Building interactive AI applications with Streamlit.
- Understanding the role of Ollama in running open-source language models locally.
- Managing Python dependencies and virtual environments.

## 🔧 Troubleshooting

**Model not found**

```bash
ollama pull gemma3
```

**Ollama connection error**

Make sure Ollama is installed and its service is running before starting the application.

**Missing Python packages**

Activate your virtual environment and run:

```bash
pip install -r requirements.txt
```

**Streamlit command not recognized**

Run the application using:

```bash
python -m streamlit run ollama.py
```

## 🔮 Future Improvements

Potential enhancements include:

- Conversation history and multi-turn chat.
- A chat-style interface with `st.chat_message`.
- Model selection from available Ollama models.
- Configurable generation parameters.
- Improved error handling and loading indicators.

## 👨‍💻 Author

**Ayush Shrivastava**

- GitHub: [@AyushShrivastava2808](https://github.com/AyushShrivastava2808)
- Project Repository: [Chatbot-using-Ollama](https://github.com/AyushShrivastava2808/Chatbot-using-Ollama)

---

⭐ If you find this project useful, consider giving the repository a star.

*Built to explore local LLMs and practical AI application development.*
