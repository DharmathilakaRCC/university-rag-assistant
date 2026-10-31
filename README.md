# 🎓 University AI Assistant – RAG Based Question Answering System

An AI-powered University Knowledge Assistant built using **Retrieval-Augmented Generation (RAG)**. The application allows users to upload university PDF documents and ask questions based on their content.

## 📌 Project Overview

This project implements a Retrieval-Augmented Generation (RAG) system that combines document retrieval with Large Language Models (LLMs) to provide context-based answers from university documents.

Users can upload multiple PDF files, process them into a searchable knowledge base, and interact with the AI assistant through a Streamlit chat interface.

## ✨ Features

- Upload multiple university PDF documents.
- Process and store documents in a knowledge base.
- Ask questions using natural language.
- Retrieve relevant document information.
- Generate answers using a local LLM.
- Display source document names and page numbers.
- Interactive chat interface using Streamlit.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| LangChain | RAG application framework |
| Streamlit | User interface |
| Ollama | Run LLMs locally |
| Llama 3.2 3B | Answer generation |
| Qwen3 Embedding 0.6B | Text embeddings |
| ChromaDB | Vector database |
| PyPDF | PDF processing |

## 🏗️ RAG Architecture

The application follows these main stages:

1. **Document Ingestion** – Upload and extract information from PDF documents.
2. **Chunking** – Divide documents into smaller text sections.
3. **Embedding** – Convert text into numerical vector representations.
4. **Vector Storage** – Store embeddings in ChromaDB.
5. **Retrieval** – Retrieve relevant document sections based on user questions.
6. **Generation** – Use the LLM to generate answers using retrieved context.

## 📂 Project Structure

```text
RAG_Project/
│
├── app.py
├── ingest.py
├── rag_pipeline.py
├── requirements.txt
├── .gitignore
│
├── data/
├── chroma_db/
└── rag_env/
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/DharmathilakaRCC/university-rag-assistant.git
```

### 2. Navigate to the project folder

```bash
cd university-rag-assistant
```

### 3. Create a virtual environment

```bash
py -3.12 -m venv rag_env
```

### 4. Activate the environment

```powershell
.\rag_env\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Install Ollama

Download Ollama from https://ollama.com/download/windows

Pull the required models:

```bash
ollama pull llama3.2:3b
ollama pull qwen3-embedding:0.6b
```

### 7. Run the application

```bash
streamlit run app.py
```

## 💬 How to Use

1. Launch the Streamlit application.
2. Upload one or more university PDF documents.
3. Click **Process Documents**.
4. Enter a question in the chat interface.
5. Receive an AI-generated answer.
6. View the retrieved source documents and page numbers.

## 🎯 Project Objective

To develop a document-based university knowledge assistant that uses Retrieval-Augmented Generation to provide relevant answers from university PDF documents.

## 👩‍💻 Developer

**Chandalee Dharmathilaka**

GitHub: https://github.com/DharmathilakaRCC

## 📚 Academic Context

Developed as part of the PUSL 3205 – Large Language Models and Generative AI practical work.