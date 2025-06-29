# Simple Langchain Chatbot

Welcome to my LangChain learning project! This repository showcases two chatbot implementations using the LangChain framework:

1. 💬 **Chatbot using Groq API with OpenAI-Compatible Model (`llama3-8b-8192`)**
2. 🤖 **Chatbot using Local Ollama with `gemma3:1b`**

These simple apps demonstrate how to use LangChain's prompt templates, output parsers, and Streamlit UI for building intelligent conversational agents.

---

## 🧠 What is LangChain?

[LangChain](https://www.langchain.com/) is a framework for developing applications powered by language models. It helps you manage prompts, chains, memory, agents, tools, and integrations with LLMs like OpenAI, Groq, and local models like Ollama.

---

## 📦 Project Structure

```

├── .env
├── app.py       # Groq API chatbot using LangChain
├── localollama.py     # Local Ollama chatbot using LangChain
├── README.md             # You're here!

````

---

## 📋 Prerequisites

- Python 3.10+
- [Streamlit](https://streamlit.io/)
- [Ollama](https://ollama.ai/) installed and `gemma3:1b` model pulled locally
- Groq API key from [Groq Cloud](https://console.groq.com/)
- LangChain and related dependencies

---

## 🛠️ Installation

```bash
git clone https://github.com/Pranay-Rokade/Simple_Langchain_Chatbot.git
cd Simple_Langchain_Chatbot

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
````

---

## 🔐 .env Configuration

Create a `.env` file in the root directory:

```env
GROQ_API_KEY=your_groq_api_key
LANGCHAIN_API_KEY=your_langchain_api_key   # (Optional: for LangSmith tracking)
```

---

## 🚀 Running the Chatbots

### 1️⃣ Groq API Chatbot

```bash
streamlit run app.py
```

This launches a chatbot using Groq's OpenAI-compatible endpoint and the `llama3-8b-8192` model.

---

### 2️⃣ Local Ollama Chatbot

Make sure Ollama is running with the required model:

```bash
ollama run gemma3:1b
```

Then start the Streamlit app:

```bash
streamlit run localollama.py
```

This uses a local LLM (Gemma) via the Ollama backend with LangChain.

---

## 🧩 Key LangChain Concepts Used

* `ChatPromptTemplate`: Defines structured prompts with role-based messages.
* `StrOutputParser`: Parses LLM responses into plain text.
* `ChatOpenAI` (with Groq): Wraps the Groq LLM endpoint.
* `Ollama`: Connects to local LLM models for private inference.
* `Streamlit`: Provides a minimal web UI for chat interaction.

---

## 📚 Future Enhancements

* Add memory to retain conversation history.
* Integrate RAG (Retrieval-Augmented Generation) for document QA.
* Enable LangSmith tracking for better debugging and monitoring.
* Extend to agent-based tasks with tools.

---

## 🙌 Acknowledgements

* [LangChain](https://github.com/langchain-ai/langchain)
* [Groq](https://console.groq.com/)
* [Ollama](https://ollama.ai/)
* [Streamlit](https://streamlit.io/)

---

## 🧠 Let's Build Smarter Apps, Together!

Feel free to fork, play around, and contribute to this repository. It’s just the beginning of a journey into the world of LLMs and intelligent apps.
