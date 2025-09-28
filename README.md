
📚 Multi-PDF Chat Agent 🤖

Developed by Aditya Goyal

Chat seamlessly with multiple PDFs using LangChain, Google Gemini, HuggingFace embeddings, and FAISS Vector DB, all wrapped inside a clean Streamlit UI.

Get fast, accurate, and natural answers from your documents — ask questions in plain language, and the AI finds + explains answers directly from your PDFs. 🔥✨

⸻

📝 Description

The Multi-PDF Chat Agent is a Streamlit-powered RAG (Retrieval-Augmented Generation) application that enables:
	•	📂 Uploading multiple PDF documents
	•	📑 Automatic text extraction + intelligent chunking
	•	🔎 Building a FAISS vector index for fast retrieval
	•	🤖 Real-time, evidence-based Q&A with ChatGPT-like answers

👉 Think of it as ChatGPT for your documents.

⸻

📊 Demo

⚡ Coming soon on Streamlit Cloud and Hugging Face Spaces. Stay tuned!

⸻

🎯 How It Works
	1.	PDF Loading → Extracts raw text from uploaded PDFs
	2.	Text Chunking → Splits into smaller sections for efficient retrieval
	3.	Embeddings → Uses HuggingFace (all-MiniLM-L6-v2) for semantic vectorization
	4.	Vector DB (FAISS) → Stores embeddings for lightning-fast similarity search
	5.	LLM (Gemini) → Generates natural answers by combining evidence with reasoning

⸻

🚀 Features
	•	✅ Multi-PDF Conversational QA
	•	✅ HuggingFace embeddings (free, unlimited, no API limits)
	•	✅ Google Gemini LLM (contextual, powerful reasoning)
	•	✅ Natural ChatGPT-like responses (no JSON clutter)
	•	✅ Evidence highlighting → know where answers came from
	•	✅ Elegant Streamlit UI with a polished design

⸻

⚙️ Requirements
	•	streamlit – interactive web app
	•	google-generativeai – Gemini integration
	•	python-dotenv – load .env configs securely
	•	langchain, langchain-community – RAG pipelines
	•	PyPDF2 – PDF text extraction
	•	faiss-cpu – vector database
	•	sentence-transformers – HuggingFace embeddings
	•	langchain-google-genai – Gemini wrapper

⸻

▶️ Installation

Clone the repository:

git clone https://github.com/Adityism/Ragbot.git
cd Ragbot

Install dependencies:

pip install -r requirements.txt

Set up environment variables (.env):

GOOGLE_API_KEY=<your-gemini-api-key>

Run the app:

streamlit run chatapp.py


⸻

💡 Usage
	1.	Upload one or more PDFs via the sidebar
	2.	Click Build Index to process them
	3.	Ask any question in plain English
	4.	Get natural answers + supporting evidence instantly

⸻

📁 Project Structure

Ragbot/
├── RAG-BOT/               # Core app
│   ├── docs/              # Uploaded PDFs
│   ├── faiss_index/       # FAISS Vector DB
│   └── chatapp.py         # Main Streamlit app
├── requirements.txt
├── .env                   # Gemini API key
└── README.md


⸻

🪪 License

Distributed under the MIT License. See LICENSE for details.

⸻

⭐ Support

If you find this project useful:
	•	🌟 Star the repo → Adityism/Ragbot
	•	🤝 Connect with me:
	•	LinkedIn
	•	GitHub

⸻

💡 Built with ❤️ by Aditya Goyal
