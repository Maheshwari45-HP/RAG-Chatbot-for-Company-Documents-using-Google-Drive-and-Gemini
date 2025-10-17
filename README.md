# 🤖 RAG Chatbot for Company Documents (Google Drive + Gemini)

**Unlock the power of your company documents with AI!**  
This workflow is a **Retrieval-Augmented Generation (RAG) chatbot** that answers employee questions based on **Google Drive documents**. It automatically indexes new or updated files into a **Pinecone vector database**, ensuring **accurate, real-time responses**.  
Powered by **Google Gemini AI** for embeddings and chat responses.  

---

## ⚙️ How It Works

1. **📂 Google Drive Triggers**  
   - Detects **new files** & **updates** in a specified folder.  

2. **📝 Automated Indexing**  
   - **Downloads** the file ✅  
   - **Loads document content** 📄  
   - **Splits content** into smaller chunks ✂️  
   - **Generates embeddings** with **Gemini AI** 💡  
   - **Indexes chunks** in **Pinecone vector database** 📊  

3. **💬 Chat Interface**  
   - Users ask a **question** ❓  
   - **AI Agent retrieves** relevant info from Pinecone 🔍  
   - Sends **context + question** to **Google Gemini Chat Model (gemini-pro)** 🤖  
   - Generates a **comprehensive answer** 🏆  
   - Uses **Window Buffer Memory** for **context-aware conversations** 🧠  

---

## 🛠️ Setup Steps

1. **🌐 Google Cloud Project & Vertex AI**  
   - Create a **Google Cloud project**  
   - Enable **Vertex AI API**  

2. **🔑 API Keys**  
   - **Google AI API Key** (Google AI Studio)  
   - **Pinecone API Key** → create index **`company-files`**  

3. **📁 Google Drive Folder**  
   - Create a **dedicated folder** for your documents  

4. **🔧 n8n Credentials**  
   - Configure:  
     - **Google Drive OAuth2**  
     - **Google Gemini (PaLM) API**  
     - **Pinecone API**  

5. **🚀 Import & Configure Workflow**  
   - **Import** into n8n  
   - Update **Google Drive Trigger nodes** to watch your folder  
   - Configure **Pinecone Vector Store nodes** to use **`company-files`** index  

---

## ⚡ Features

- 🔹 **Real-time indexing** of new or updated documents  
- 🔹 **Vector retrieval** for **precise answers**  
- 🔹 **Context-aware conversation** using memory nodes 🧠  
- 🔹 Powered by **Google Gemini AI** for embeddings & chat 💡  
- 🔹 Fully automated workflow in **n8n** ⚙️  

---

 
