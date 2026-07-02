# Setup Guide

## Prerequisites

- Docker
- n8n (latest)
- Git
- ngrok Tunnel
- Google Account
- Telegram Bot
- Groq API Key
- Hugging Face API Key
- OpenRouter API Key (optional)
- Pinecone Account
- SearchAPI / Tavily (optional)

---

## Installation

### 1. Clone Repository

```bash
git clone https://github.com/<username>/n8n-ai-workflows.git
cd n8n-ai-workflows
```

---

### 2. Start n8n

```bash
docker run -d \
--name n8n \
-p 5678:5678 \
-v D:\DevFiles\n8n-data:/home/node/.n8n \
docker.n8n.io/n8nio/n8n
```

---

### 3. Start ngrok Tunnel

```bash
ngrok tunnel --url http://localhost:5678
```

Copy the generated URL.

---

### 4. Configure Environment

Set:

- WEBHOOK_URL
- N8N_HOST
- N8N_PROTOCOL

Restart the Docker container.

---

### 5. Import Workflows

Import every JSON file from the `workflows/` folder.

---

### 6. Configure Credentials

Reconnect:

- Telegram
- Gmail
- Google Calendar
- Google Contacts
- Google Drive
- Google Sheets
- Groq
- Hugging Face
- Pinecone
- SearchAPI
- Tavily
- OpenRouter (optional)

---

### 7. Activate Workflows

Enable the workflows you want to use.

---

## Verification

The assistant should now be able to:

- Chat via Telegram
- Manage Gmail
- Manage Calendar
- Search Contacts
- Generate Content
- Generate AI Video Prompts
- Screen Resumes
- Update the Pinecone Knowledge Base