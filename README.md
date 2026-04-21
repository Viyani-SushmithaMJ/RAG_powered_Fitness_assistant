# RAG_powered_Fitness_assistant

A RAG based fitness and wellness virtual assistant that provides users with dynamic, personalized, and actionable recommendations and tips on fitness routine and nutrition intake.
# 📚 AI-Powered Document Question Answering System (RAG with FAISS + LLM)

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Transformers](https://img.shields.io/badge/Transformers-HuggingFace-yellow)
![FAISS](https://img.shields.io/badge/VectorDB-FAISS-orange)
![SentenceTransformers](https://img.shields.io/badge/Embeddings-SBERT-green)
![PyMuPDF](https://img.shields.io/badge/PDF%20Parsing-PyMuPDF-purple)

---

## 🚀 Project Overview

This project builds a **Retrieval-Augmented Generation (RAG) system** that allows users to ask questions from a collection of PDF documents and receive **context-aware, human-like answers**.

It combines:
- 🔍 Semantic Search (FAISS)
- 🧠 Dense Embeddings (SentenceTransformers)
- 🤖 Large Language Model (GPT-Neo)
- 📄 PDF Knowledge Base (PyMuPDF)

---

## 🧠 Key Features

- 📄 PDF document ingestion and text extraction
- ✂️ Smart chunking of documents
- 🔎 Semantic search using embeddings
- ⚡ FAISS vector database for fast retrieval
- 🤖 GPT-Neo-based answer generation
- 🎯 Relevance filtering using similarity threshold
- 📉 Response quality filtering (perplexity + similarity)
- ⏱️ Response time tracking
- 📊 Evaluation metrics (similarity score, perplexity score)

---

## 🏗️ System Architecture

```text
PDF Documents
     ↓
Text Extraction (PyMuPDF)
     ↓
Chunking (500-word segments)
     ↓
Embedding Model (SentenceTransformers)
     ↓
Vector Database (FAISS Index)
     ↓
Query Embedding
     ↓
Semantic Retrieval (Top-K chunks)
     ↓
Context + Query → LLM (GPT-Neo)
     ↓
Filtered High-Quality Answer

```
## ⚙️ Installation

pip install transformers sentence-transformers faiss-cpu PyMuPDF

📊 Evaluation Metrics
⏱️ Response Time

📈 Similarity Score

Measures semantic alignment between query and response

📉 Perplexity Score
Measures response confidence and fluency

📌 Sample Output
User Query:
what are the expert tips for beginners at gym?
System Response:
Retrieves relevant PDF chunks
Generates contextual answer using GPT-Neo
Filters response using similarity + perplexity checks

📊 Example Metrics
Metric	Value
Similarity Score	~0.59
Perplexity Score	~8.87
Response Time	~39s

🧰 Tech Stack
Python 🐍
HuggingFace Transformers 🤗
SentenceTransformers 🔎
FAISS (Vector Search) ⚡
PyMuPDF 📄
GPT-Neo 🤖

🔥 Key Capabilities

Semantic document search

Context-aware question answering

Retrieval-Augmented Generation (RAG)

Response filtering for quality control

Scalable vector database search

📌 Future Improvements

🧠 Hybrid search (BM25 + embeddings)
