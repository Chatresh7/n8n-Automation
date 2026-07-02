# 🤖 n8n Automation Hub

> A collection of intelligent automation workflows built using **n8n**, integrating AI, messaging platforms, Google Workspace, vector databases, and cloud services to automate real-world tasks.

![n8n](https://img.shields.io/badge/n8n-Automation-EA4B71?style=for-the-badge&logo=n8n)
![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker)
![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=for-the-badge&logo=telegram)
![Google Workspace](https://img.shields.io/badge/Google-Workspace-4285F4?style=for-the-badge&logo=google)
![Groq](https://img.shields.io/badge/Groq-AI-black?style=for-the-badge)
![Pinecone](https://img.shields.io/badge/Pinecone-VectorDB-0E9F6E?style=for-the-badge)

---

# 📌 Overview

This repository contains multiple production-ready **n8n workflows** that automate repetitive tasks using AI and modern cloud services.

The workflows demonstrate integrations with:

- 🤖 AI Agents
- 📧 Gmail
- 📅 Google Calendar
- 👥 Google Contacts
- 📂 Google Drive
- 📊 Google Sheets
- 💬 Telegram
- 🧠 Pinecone Vector Database
- 🎤 Speech-to-Text (Groq Whisper)
- 🔍 AI Search APIs
- ☁️ Docker + Cloudflare/ngrok

---

# 🚀 Features

## 🤖 AI Assistant

- Conversational AI
- Voice & text support
- Memory-enabled conversations
- Tool calling

---

## 📧 Gmail Automation

- Read emails
- Search emails
- Summarize inbox
- Draft replies
- Send emails
- Filter promotional emails

---

## 📅 Google Calendar

- Create events
- Update events
- Delete events
- Check schedules
- Natural language scheduling

Example:

> "Schedule Yoga tomorrow at 3 PM."

---

## 👥 Google Contacts

- Search contacts
- Add contacts
- Update contacts

---

## ✍️ Content Generation

- Social media posts
- Blog articles
- Captions
- Scripts
- AI prompts
- Marketing content

---

## 🎥 AI Video Prompt Generator

Generate structured prompts for AI video models.

Includes:

- Cinematic prompts
- Before/After transformations
- VEO3-ready prompts

---

## 📄 Resume Screening

AI-powered ATS workflow that can:

- Parse resumes
- Extract skills
- Match candidates
- Score resumes

---

## 🧠 RAG Knowledge Base

- Upload documents
- Split into chunks
- Generate embeddings
- Store in Pinecone
- Semantic search

---

## 🎤 Voice AI

Supports voice messages using:

- Groq Whisper
- Speech-to-Text
- AI responses

---

# 📂 Repository Structure

```
n8n-Automation/
│
├── workflows/
│   ├── Telegram.json
│   ├── Email-Agent.json
│   ├── Calendar-Agent.json
│   ├── Resume-Screener.json
│   ├── Video-Generator.json
│   └── ...
│
├── screenshots/
│
├── docs/
│   ├── setup.md
│   ├── architecture.md
│   └── integrations.md
│
├── README.md
├── LICENSE
└── .gitignore
```

---

# 🏗️ Architecture

```
                  Telegram
                      │
                      ▼
             Telegram Trigger
                      │
         Voice / Text Detection
              │             │
              ▼             ▼
      Groq Whisper      Text Input
              │
              ▼
        Supervisor Agent
              │
     ┌────────┼────────┐
     ▼        ▼        ▼
 Email     Calendar  Contacts
     │
     ▼
 Content Agent
     │
     ▼
 Video Generator
```

---

# 🛠️ Tech Stack

### Workflow Automation

- n8n

### AI

- Groq
- Google Gemini
- OpenRouter
- Hugging Face

### Databases

- Pinecone
- Google Sheets

### Google Workspace

- Gmail
- Calendar
- Drive
- Contacts

### Messaging

- Telegram Bot API

### Infrastructure

- Docker
- Cloudflare Tunnel
- ngrok

---

# 📦 Setup

See:

- 📖 `docs/setup.md`
- 🏗️ `docs/architecture.md`
- 🔌 `docs/integrations.md`

---

# 📷 Screenshots

Add workflow screenshots inside the `screenshots/` directory.

Example:

```
screenshots/
    telegram-workflow.png
    ai-agent.png
    resume-screener.png
```

---

# 🔐 Security

This repository **does not include**:

- API Keys
- OAuth Tokens
- Credentials
- Environment Variables

Configure your own credentials after importing the workflows.

---

# 📥 Importing Workflows

1. Open n8n.
2. Click **Import Workflow**.
3. Select any JSON file from the `workflows/` directory.
4. Configure credentials.
5. Activate the workflow.

---

# 🤝 Contributing

Contributions, improvements, and suggestions are welcome.

Feel free to open:

- Issues
- Feature requests
- Pull requests

---

# ⭐ Support

If you found this repository useful:

⭐ Star the repository

🍴 Fork it

💡 Share it with others

---

# 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Chatresh Konchada**

- GitHub: https://github.com/Chatresh7
- LinkedIn: https://www.linkedin.com/in/chatresh-konchada/

---

> Built with ❤️ using n8n, AI, and automation.
