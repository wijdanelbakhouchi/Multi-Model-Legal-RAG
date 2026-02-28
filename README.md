# ⚖️ JuristAI-Maroc: Legal RAG Assistant
JuristAI-Maroc is an intelligent legal assistant designed to answer questions based on Moroccan law documents. It leverages a RAG (Retrieval-Augmented Generation) architecture to provide precise, context-aware answers by querying a specialized vector database of Moroccan legal texts.
## 🚀 Key Features
- **Multi-Model Comparison:** Evaluates and compares the performance of Mistral 7B (4-bit) and TinyLlama-1.1B for legal question-answering tasks.
- **Vector Database (ChromaDB):** Uses HuggingFaceEmbeddings (all-MiniLM-L6-v2) to store and retrieve legal document segments efficiently.
- **Performance Benchmarking:** Comprehensive evaluation of models based on F1-Score, Sémantique (Cosine Similarity), and Inference Time.
- **User-Friendly Interface:** Two distinct Gradio chat interfaces for interacting with the AI assistants directly.
- **Cloud Persistence:** Seamless integration with Google Drive for persistent storage of the ChromaDB vector database.

## 🛠️ Tech Stack
- *Languages:* Python
- *Frameworks:* LangChain, Gradio
- *LLMs:* Mistral-7B-Instruct-v0.2 (via bitsandbytes 4-bit quantization), TinyLlama-1.1B-Chat-v1.0
- *Vector Store:* ChromaDB
- *Hardware Optimization:* CUDA-based GPU acceleration (optimized for T4 GPUs)

## 📊 Benchmarking Highlights

The project includes an evaluation module that generates performance heatmaps and comparison tables, measuring:
- Accuracy (Exact Match)
- Lexical Overlap (F1-Token & Rouge-L)
- Inference Speed (tokens/sec)
