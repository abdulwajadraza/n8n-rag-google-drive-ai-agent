📚 n8n RAG System – Google Drive AI Knowledge Assistant
🚀 Project Overview

This project implements a Retrieval-Augmented Generation (RAG) system using n8n.

The system:

Downloads company documents from Google Drive

Converts them into embeddings

Stores them in a Supabase Vector Store

Uses an AI Agent to answer user queries based only on company documents

🧠 Architecture

1️⃣ Trigger workflow execution
2️⃣ Download files from Google Drive
3️⃣ Load and chunk documents
4️⃣ Generate embeddings (Google Gemini)
5️⃣ Store embeddings in Supabase Vector Store
6️⃣ AI Agent retrieves relevant chunks
7️⃣ Answer user queries using RAG

🛠️ Modules Used
🔹 Google Drive

Downloads company documents automatically.

🔹 Default Data Loader

Processes and chunks documents.

🔹 Google Gemini Embeddings

Generates vector embeddings for semantic search.

🔹 Supabase Vector Store

Stores embeddings for retrieval.

🔹 AI Agent

Handles user queries.

🔹 Google Gemini Chat Model

Generates final answer.

🔹 Postgres Chat Memory

Stores conversation history.

🎯 Key Features

✅ Fully automated document ingestion
✅ Vector-based semantic search
✅ Conversational memory
✅ Scalable architecture
✅ No hallucination (answers from documents only)

🔐 Environment Variables

Create .env file using .env.example:

GOOGLE_API_KEY=
SUPABASE_URL=
SUPABASE_SERVICE_ROLE_KEY=
POSTGRES_CONNECTION_STRING=

▶️ How to Use

Import workflow.json into n8n

Configure credentials

Set environment variables

Execute workflow

Start asking questions

📸 Architecture Diagram

👨‍💻 Author

Abdul Wajad Raza
AI Developer | Automation Enthusiast

🏷️ Tags

RAG, n8n, AI Agent, Vector Database, Supabase, Google Gemini, Automation