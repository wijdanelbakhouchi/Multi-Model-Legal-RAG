# Multi-Model Legal RAG (Retrieval-Augmented Generation)

<p align="left">
  <img src="https://img.shields.io/badge/STATUS-EDUCATIONAL%20PROJECT-0078D4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/ARCH-RAG%20PIPELINE-E87B1E?style=for-the-badge" />
  <img src="https://img.shields.io/badge/LLM-GEMINI%20|%20GROQ-606060?style=for-the-badge" />
</p>

<p align="left">
  <img src="https://img.shields.io/badge/VECTOR%20DB-CHROMA%20DB-555555?style=for-the-badge" />
  <img src="https://img.shields.io/badge/FRAMEWORK-LANGCHAIN%20|%20STREAMLIT-0078D4?style=for-the-badge" />
</p>

> **A sophisticated legal assistant leveraging Retrieval-Augmented Generation (RAG) to provide accurate, context-aware answers from complex legal documentation using multi-model orchestration.**
## Key Features
- **Multi-Model Comparison:** Evaluates and compares the performance of Mistral 7B (4-bit) and TinyLlama-1.1B for legal question-answering tasks.
- **Vector Database (ChromaDB):** Uses HuggingFaceEmbeddings (all-MiniLM-L6-v2) to store and retrieve legal document segments efficiently.
- **Performance Benchmarking:** Comprehensive evaluation of models based on F1-Score, Sémantique (Cosine Similarity), and Inference Time.
- **User-Friendly Interface:** Two distinct Gradio chat interfaces for interacting with the AI assistants directly.
- **Cloud Persistence:** Seamless integration with Google Drive for persistent storage of the ChromaDB vector database.

## Tech Stack
- *Languages:* Python
- *Frameworks:* LangChain, Gradio
- *LLMs:* Mistral-7B-Instruct-v0.2 (via bitsandbytes 4-bit quantization), TinyLlama-1.1B-Chat-v1.0
- *Vector Store:* ChromaDB
- *Hardware Optimization:* CUDA-based GPU acceleration (optimized for T4 GPUs)

## Benchmarking Highlights

The project includes an evaluation module that generates performance heatmaps and comparison tables, measuring:
- Accuracy (Exact Match)
- Lexical Overlap (F1-Token & Rouge-L)
- Inference Speed (tokens/sec)
