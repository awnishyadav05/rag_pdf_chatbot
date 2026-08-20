# RAG Document Q&A

This project is a simple implementation of a **Retrieval-Augmented Generation (RAG)** system using LangChain and Google Gemini.

The main idea is to upload/read documents and ask questions about their content. Instead of directly asking the LLM, the system first searches the relevant information from the documents and then uses that information to generate the answer.

## What I Used

- Python
- LangChain
- Google Gemini
- Google Generative AI Embeddings
- ChromaDB
- PyPDF
- Docx2txt
- Jupyter Notebook / Google Colab

## How It Works

The project follows these steps:

1. Load PDF and DOCX files
2. Split the documents into smaller chunks
3. Create embeddings for the chunks
4. Store the embeddings in ChromaDB
5. Search for relevant chunks when a question is asked
6. Pass the retrieved information to Gemini
7. Generate the final answer

```text
Documents
   ↓
Load Documents
   ↓
Split into Chunks
   ↓
Create Embeddings
   ↓
ChromaDB
   ↓
Retriever
   ↓
Relevant Context
   ↓
Gemini
   ↓
Answer
