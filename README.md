# Legal-RAG-System
# ⚖️ Legal Document Q&A using RAG (Retrieval-Augmented Generation)

## 📌 Project Overview
This project implements a Retrieval-Augmented Generation (RAG) system to efficiently extract and answer queries from large-scale legal documents. The system combines document retrieval with language generation to provide accurate, context-aware responses.

It is designed to assist legal professionals in quickly finding relevant clauses and insights from complex legal texts.

---

## 🎯 Business Objective
Legal teams often deal with large volumes of contracts and policies, making manual search time-consuming and inefficient.

The objective of this project is to:
- Retrieve relevant legal information efficiently
- Provide accurate answers to legal queries
- Reduce time spent on document review
- Improve decision-making using data-driven insights

---

## 📂 Dataset Description
The dataset consists of legal documents stored as text files across multiple categories:

- **contractnli** → Confidentiality & NDA agreements  
- **cuad** → Contracts with annotated clauses  
- **maud** → Merger & acquisition agreements  
- **privacy_qa** → Privacy policies with Q&A format  

Additionally, benchmark datasets (JSON format) contain:
- Questions  
- Ground truth answers  
- Source references  

---

## ⚙️ Methodology

### 🔹 1. Document Loading
- Loaded text documents from multiple folders
- Structured data for processing

### 🔹 2. Text Chunking
- Split documents into smaller chunks for better retrieval

### 🔹 3. Embedding Generation
- Converted text into vector embeddings using LLM-based models

### 🔹 4. Vector Database
- Stored embeddings using FAISS for fast similarity search

### 🔹 5. Retrieval System
- Retrieved relevant document chunks based on query

### 🔹 6. Response Generation
- Used LLM (via LangChain / LlamaIndex) to generate contextual answers

---

## 🧠 Tech Stack
- Python
- LangChain / LlamaIndex
- FAISS (Vector Database)
- OpenAI / LLM APIs
- Pandas, NumPy

---

## 📊 Key Features
- Efficient semantic search across legal documents
- Context-aware answer generation
- Handles multiple document types
- Scalable architecture for large datasets

---

## 📈 Results & Insights
- Successfully retrieved relevant legal clauses
- Generated accurate responses to benchmark questions
- Improved efficiency in legal document analysis
- Demonstrated strong retrieval + generation pipeline

---

## 📁 Project Structure

├── data/
│ ├── corpus/
│ │ ├── contractnli/
│ │ ├── cuad/
│ │ ├── maud/
│ │ └── privacy_qa/
│ ├── benchmarks/
│ │ ├── contractnli.json
│ │ ├── cuad.json
│ │ ├── maud.json
│ │ └── privacy_qa.json
│
├── outputs/
│ ├── faiss_index/
│ ├── processed_data/
│ └── results/
│
├── notebooks/
│ └── RAG_Legal_Docs.ipynb
│
├── README.md


---

## 🚀 Future Improvements
- Improve retrieval accuracy using advanced embeddings
- Add UI for interactive querying
- Integrate real-time legal databases
- Optimize response generation using fine-tuned models

---

## ⭐ Conclusion
This project demonstrates how combining retrieval systems with generative AI can significantly improve information access in complex domains like legal analytics.
