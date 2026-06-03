

# 🤖 AI Agent Workflow (n8n + Groq + Google Drive)

This project is an **AI-powered chat agent workflow built in n8n**.  
It uses a Large Language Model (LLM) via Groq, memory buffer, and Google Drive tool integration to answer queries and interact with files.

---

## 🚀 Features

- 💬 Chat-based AI agent (triggered via chat message)
- 🧠 Memory support (conversation context retention)
- 🤖 LLM integration using Groq (LLaMA 3.3 70B)
- 📁 Google Drive file & folder search tool
- 🔗 Modular LangChain-based architecture

---

## 🧩 Workflow Nodes

### 1. Chat Trigger
Starts workflow when a user sends a message.

### 2. AI Agent
Core reasoning engine that processes input and coordinates tools.

### 3. Groq Chat Model
- Model: `llama-3.3-70b-versatile`
- Provides LLM reasoning and responses

### 4. Simple Memory Buffer
Stores short-term conversation history for context-aware responses.

### 5. Google Drive Tool
Searches files and folders in Google Drive using connected account.

---

## ⚙️ Requirements

- n8n installed (desktop or self-hosted)
- Groq API key
- Google Cloud OAuth credentials (for Drive access)
- Internet connection

![image alt](https://github.com/BasitMunir16/Ai-drive-assistant-/blob/6bb42dfa629fc90fc1381cf16265247b8a7807bd/Screenshot%202026-06-03%20192945.png)
---

## 🔐 Setup Instructions

### 1. Import Workflow
- Open n8n
- Click **Import Workflow**
- Paste the JSON file

### 2. Configure Credentials

#### Groq
- Go to Credentials
- Add Groq API Key
- Select it in **Groq Chat Model node**

#### Google Drive
- Create OAuth2 credentials in Google Cloud Console
- Enable Google Drive API
- Connect in n8n credentials panel

---

## 🧠 How It Works

1. User sends a chat message
2. Chat Trigger activates workflow
3. AI Agent processes request
4. LLM generates reasoning via Groq
5. Memory provides context (if needed)
6. Google Drive tool is used if file search is required
7. Final response is returned to user

---

## 📌 Use Cases

- AI assistant chatbot
- Personal file search assistant
- Knowledge base explorer
- Automation + AI hybrid agent

---

## 🛠 Tech Stack

- n8n
- LangChain nodes
- Groq LLM API
- Google Drive API

---

## ⚠️ Notes

- Make sure credentials are correctly configured before activation
- Do not expose API keys in shared workflows
- Workflow is currently set to **inactive by default**

---

## 👤 Author

Built using n8n AI Agent framework
