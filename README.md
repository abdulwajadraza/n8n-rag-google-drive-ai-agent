# 📚 n8n RAG System – Google Drive AI Knowledge Assistant

A fully automated **Retrieval-Augmented Generation (RAG)** system built using **n8n**, **Supabase Vector Store**, and **Google Gemini AI**.

This system downloads company documents from Google Drive, converts them into embeddings, stores them in a vector database, and answers user queries strictly based on those documents.

---

## 🚀 Project Overview

This workflow automates:

1. 📥 Downloading documents from Google Drive  
2. 📄 Processing & chunking documents  
3. 🧠 Generating embeddings using Google Gemini  
4. 🗄️ Storing embeddings in Supabase Vector Store  
5. 🤖 AI Agent retrieving relevant content  
6. 💬 Answering user queries using RAG  
7. 🧾 Maintaining chat history with Postgres Memory  

This ensures accurate, document-grounded responses with reduced hallucination.

---

## 🏗️ System Architecture

```
User Query
    ↓
AI Agent
    ↓
Vector Search (Supabase)
    ↓
Relevant Document Chunks
    ↓
Gemini Chat Model
    ↓
Final Answer
```

Document Ingestion Flow:

```
Google Drive → Data Loader → Embeddings (Gemini) → Supabase Vector Store
```

---

## 🛠️ Technologies Used

- **n8n** (Workflow Automation)
- **Google Drive API**
- **Google Gemini (Embeddings + Chat Model)**
- **Supabase (Vector Store)**
- **PostgreSQL (Chat Memory)**
- **RAG Architecture**

---

## 🔧 Workflow Components

### 1️⃣ Trigger
Manual workflow execution or chat trigger.

### 2️⃣ Google Drive Node
Downloads company documents automatically.

### 3️⃣ Default Data Loader
Processes and splits documents into chunks.

### 4️⃣ Google Gemini Embeddings
Creates vector embeddings for semantic similarity search.

### 5️⃣ Supabase Vector Store
Stores document embeddings for retrieval.

### 6️⃣ AI Agent
Handles user queries and retrieves relevant context.

### 7️⃣ Google Gemini Chat Model
Generates final answers grounded in retrieved content.

### 8️⃣ Postgres Chat Memory
Maintains conversational history.

---

## 🎯 Key Features

- ✅ Automated document ingestion
- ✅ Vector-based semantic search
- ✅ Context-aware AI responses
- ✅ Conversational memory support
- ✅ Reduced hallucination
- ✅ Enterprise-ready architecture
- ✅ Scalable and modular design

---

## 🔐 Environment Variables

Create a `.env` file based on `.env.example`:

```env
GOOGLE_API_KEY=your_google_api_key
SUPABASE_URL=your_supabase_url
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
POSTGRES_CONNECTION_STRING=your_postgres_connection
```

---

## ▶️ How to Use

1. Import `workflow.json` into n8n
2. Configure credentials (Google Drive, Supabase, Gemini)
3. Set environment variables
4. Execute the document ingestion workflow
5. Start querying via chat interface

---

## 📸 Architecture Diagram

Add your workflow screenshot here:

```
![Architecture](architecture.png)
```

---

## 📦 Repository Structure

```
.
├── workflow.json
├── architecture.png
├── .env.example
├── README.md
└── LICENSE
```

---

## 📈 Real-World Use Cases

- Company internal knowledge assistant
- HR policy Q&A bot
- Legal document assistant
- Research paper search system
- Enterprise documentation chatbot

---

## 👨‍💻 Author

**Abdul Wajad Raza**  
AI Developer | Automation Enthusiast | RAG Systems Builder  

---

## 🏷️ Tags

`RAG` `n8n` `AI Agent` `Vector Database` `Supabase` `Google Gemini` `Automation` `LLM` `Enterprise AI`

---

## ⭐ If you find this project useful, consider giving it a star!
