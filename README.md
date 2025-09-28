# 📚 Multi-PDF Chat Agent 🤖

**Developed by [Aditya Goyal](https://github.com/Adityism)**

Experience the next generation of document intelligence: Chat with multiple PDFs in natural language, powered by LangChain, Google Gemini, HuggingFace Embeddings, and FAISS Vector DB—all wrapped in a polished Streamlit UI.

> **Ask questions in plain English. Get fast, accurate, and context-rich answers—directly from your documents.**  
> _Perfect for research, legal, academics, business, or any scenario where insights from multiple PDFs matter!_

---

## 🏗️ Architecture

<img src="img/Architecture.jpg" alt="Project Flow Architecture" width="100%">

<details>
<summary>Show Architecture Description</summary>

The flow for answering your questions with evidence from multiple PDFs is visualized above:

1. **Upload PDFs** → Add any number of documents.
2. **Text Chunking** → Each PDF is split into manageable, context-rich chunks.
3. **Embeddings** → Each chunk is converted to a semantic vector using HuggingFace models.
4. **Vector Store (FAISS/Pinecone)** → Efficiently indexes and stores all vectors.
5. **Ask a Question** → User submits a natural language query.
6. **Embed the Question** → The query is transformed into a vector and compared against the knowledge base.
7. **Semantic Search & LLM** → The best-matching chunks are sent to the LLM (Google Gemini, HuggingFace, or Open Source) for answer generation.
8. **Get Natural Answer** → Receive a clear, evidence-based, conversational reply with references.

</details>

---

## 📝 Overview

The **Multi-PDF Chat Agent** is a robust Streamlit-powered Retrieval-Augmented Generation (RAG) application that empowers you to:

- 📂 **Upload** multiple PDF documents.
- 📑 **Extract** and intelligently chunk text from these PDFs.
- 🔎 **Build** a FAISS vector index for ultra-fast semantic search.
- 🤖 **Chat** with your PDFs: Real-time, evidence-based Q&A with ChatGPT-like responses, referencing the actual sources.

> **Think of it as your personal ChatGPT for all your documents!**

---

## 🚀 Features

- ✅ **Multi-PDF Conversational QA** — Chat with several PDFs at once.
- ✅ **Free, Unlimited HuggingFace Embeddings** — No API limits!
- ✅ **Google Gemini LLM** — Advanced, contextual answers.
- ✅ **Natural, JSON-free responses** — Clean, conversational outputs.
- ✅ **Evidence Highlighting** — See exactly where answers came from.
- ✅ **Streamlit UI** — Modern, minimal, and intuitive.
- ✅ **Privacy-First** — Your documents never leave your machine.

---

## 🎯 How It Works

1. **PDF Loading** → Extracts raw text from any uploaded PDFs.
2. **Text Chunking** → Splits content into context-aware segments.
3. **Embeddings** → Uses HuggingFace `all-MiniLM-L6-v2` for semantic vectorization.
4. **Vector DB (FAISS)** → Stores embeddings for lightning-fast similarity search.
5. **LLM (Gemini)** → Generates human-like answers by fusing evidence and reasoning.

---

## 📊 Demo

**Coming soon!**  
Deployments on [Streamlit Cloud](https://streamlit.io/cloud) and [Hugging Face Spaces](https://huggingface.co/spaces) are in progress. Stay tuned for live demos and one-click launches!

---

## ⚙️ Requirements

- `streamlit` — Interactive web app
- `google-generativeai` — Gemini integration
- `python-dotenv` — Securely loads .env configs
- `langchain`, `langchain-community` — RAG pipelines
- `PyPDF2` — PDF text extraction
- `faiss-cpu` — Vector database
- `sentence-transformers` — HuggingFace embeddings
- `langchain-google-genai` — Gemini wrapper

---

## ▶️ Installation

#### 1. Clone the repository

```bash
git clone https://github.com/Adityism/Ragbot.git
cd Ragbot
```

#### 2. Install dependencies

```bash
pip install -r requirements.txt
```

#### 3. Set up environment variables

Create a `.env` file with your [Google Gemini API key](https://ai.google.dev/):

```
GOOGLE_API_KEY=<your-gemini-api-key>
```

#### 4. Run the app

```bash
streamlit run chatapp.py
```

---

## 💡 Usage

1. **Upload** one or more PDFs via the sidebar.
2. **Click “Build Index”** to process and embed them.
3. **Ask any question** in plain English.
4. **Get instant, natural answers** with supporting evidence and PDF references.

---

## 📁 Project Structure

```
Ragbot/
├── RAG-BOT/               # Core app logic
│   ├── docs/              # Uploaded PDFs
│   ├── faiss_index/       # FAISS Vector DB files
│   ├── img/               # Images (including Architecture.jpg)
│   └── chatapp.py         # Main Streamlit app
├── requirements.txt
├── .env                   # Gemini API key (not committed)
└── README.md
```

---

## 🪪 License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

## ⭐ Support

If you find this project helpful:

- 🌟 **Star this repo**: [Adityism/Ragbot](https://github.com/Adityism/Ragbot)
- 🤝 **Connect with me**:
  - [LinkedIn](https://www.linkedin.com/in/aditya-goyal-2041)
  - [GitHub](https://github.com/Adityism)

---

## 💡 Built with ❤️ by Aditya Goyal
