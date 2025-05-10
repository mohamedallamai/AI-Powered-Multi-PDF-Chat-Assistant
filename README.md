# Chat with Multiple PDFs

An AI-powered PDF assistant built with **LangChain**, **Chroma**, **LLMs**, and **Streamlit**. Upload one or more PDFs, ask questions in natural language, and get accurate, context-aware answers directly from your documents — with full session history and model flexibility.

---

## ✨ Features

* **Multi-PDF Upload**: Load and manage multiple documents per chat session.
* **Intelligent Text Extraction**: Parses and chunks documents for optimal retrieval.
* **Embedding Choice**: Use **OpenAI** or **Gemini** (Google) for vector embeddings.
* **LLM Choice**: Choose between **ChatGPT (GPT-3.5)** or **Gemini 2.0** chat models.
* **Conversational Memory**: Retains context across questions within a session.
* **Per-Session Vectorstores**: Uses **Chroma DB** to store embeddings per session.
* **Session Management**: Create, select, or delete chat sessions with uploaded PDFs.
* **Secure & Configurable**: Uses `.env` for API keys and secrets.

---

## 📦 Tech Stack

| Layer            | Technology                             |
| ---------------- | -------------------------------------- |
| Frontend         | Streamlit                              |
| Document Parsing | PyPDF2                                 |
| LLM Integration  | LangChain (OpenAI + Gemini support)    |
| Vector Store     | Chroma DB                              |
| Embeddings       | OpenAI or Google Generative AI         |
| Memory Handling  | LangChain's `ConversationBufferMemory` |
| File Management  | Native Python + JSON                   |

---

## 📂 Folder Structure

```
.
├── chat-sessions.py         # Main Streamlit app
├── htmlTemplates.py         # HTML styling for UI
├── sessions/                # Saved chat sessions and PDFs
├── chroma_db/               # Chroma vector databases per session
├── .env                     # Your actual API keys (not committed)
├── .env.example             # Example env file with required keys
├── .gitignore               # Files/folders to exclude from version control
├── venv/                    # Python virtual environment
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation

```

---

## ⚙️ Configuration Options

Inside the app (sidebar):

* **Embeddings Model**: Choose between `OpenAI` and `Gemini`
* **Chat Model**: Choose between `ChatGPT` and `Gemini`
* **Session Management**: Create/delete sessions with stored chat and PDF history
* **Download Uploaded PDFs**: Quick access to files per session

---

## ✍️ Prompt Behavior

The app uses a carefully structured prompt to guide the assistant:

* Answers **only** based on the uploaded PDFs
* Responses are concise, bullet-structured or paragraph-form
* Maintains the original **language and style** of the documents

---

## ✅ Example Use Cases

* Legal document Q\&A
* Academic paper summarization
* Policy or contract review
* Customer support for manuals or guides
* Multi-document research assistant

---

## 📘 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙋‍♂️ Acknowledgements

* [LangChain](https://github.com/langchain-ai/langchain)
* [Streamlit](https://streamlit.io/)
* [Chroma](https://www.trychroma.com/)
* [OpenAI](https://platform.openai.com/)
* [Google Generative AI](https://ai.google.dev/)

---
