# Mini RAG Chatbot

A Retrieval-Augmented Generation (RAG) chatbot built using **Streamlit**, **LangChain**, **Google Gemini**, **Hugging Face Embeddings**, **FAISS**, and **ChromaDB**.

The application allows users to upload PDF documents, create a vector database, and ask questions about the document using Google's Gemini LLM.

---

## Features

- Upload PDF documents
- Extract text using PyPDF
- Split documents into chunks
- Generate embeddings using Hugging Face
- Store embeddings using:
  - FAISS
  - ChromaDB
- Ask questions using Google Gemini
- Interactive Streamlit interface

---

## Tech Stack

- Python
- Streamlit
- LangChain
- Google Gemini API
- HuggingFace Sentence Transformers
- FAISS
- ChromaDB
- PyPDF

---

# Project Structure

```text
Mini_RAG_Chatbot/
│
├── app.py
├── .env
├── requirements.txt
│
├── data/
│
├── database/
│
├── utils/
│   ├── loader.py
│   ├── splitter.py
│   ├── embeddings.py
│   ├── vectorstore.py
│   └── rag_chain.py
│
├── test_loader.py
├── test_splitter.py
├── test_embedding.py
├── test_vectorstore.py
├── test_faiss.py
├── test_chroma.py
├── test_gemini.py
└── test_rag.py
```

---

# Installation

## 1. Clone Repository

```bash
git clone https://github.com/tarushibahl/Mini_RAG_Chatbot.git

cd Mini_RAG_Chatbot
```

---

## 2. Create Virtual Environment

### Windows

```cmd
python -m venv rag_env
```

Activate

```cmd
rag_env\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv rag_env
```

Activate

```bash
source rag_env/bin/activate
```

---

## 3. Install Dependencies

Windows

```cmd
pip install -r requirements.txt
```

macOS / Linux

```bash
pip install -r requirements.txt
```

---

## 4. Configure Gemini API

Create a `.env` file.

```env
GOOGLE_API_KEY=YOUR_API_KEY
```

Generate your API key from:

https://aistudio.google.com/app/api-keys

---

## 5. Add PDF

Place your PDF inside:

```text
data/
```

Example:

```text
data/
    sample.pdf
```

---

## 6. Run Application

Windows

```cmd
streamlit run app.py
```

macOS / Linux

```bash
streamlit run app.py
```

Open

```
http://localhost:8501
```

---

# Workflow

1. Upload PDF
2. Load document
3. Split into chunks
4. Generate embeddings
5. Create FAISS/Chroma database
6. Ask questions
7. Gemini generates answers using document context

---

# Libraries Used

- Streamlit
- LangChain
- LangChain Community
- LangChain Google GenAI
- HuggingFace Embeddings
- Sentence Transformers
- FAISS
- ChromaDB
- PyPDF
- Python Dotenv

---

# Future Improvements

- Multiple PDF support
- Chat history
- OCR support
- Hybrid Search
- Citation generation
- Docker deployment
- Authentication
- Cloud deployment

---

# Author

**Tarushi Bahl**

GitHub:
https://github.com/tarushibahl