# System Architecture

## High-Level Architecture

```
                    Telegram
                        │
                        ▼
              Telegram Trigger
                        │
             Voice / Text Detection
                │              │
                │              ▼
                │         Text Input
                ▼
        Voice Transcription
          (Groq Whisper)
                │
                ▼
         Supervisor AI Agent
                │
      ┌─────────┼──────────┐
      │         │          │
      ▼         ▼          ▼
 Email Agent Calendar Contacts
      │
      ▼
 Content Creator
      │
      ▼
 Video Generator

                │
                ▼
           Telegram Reply
```

---

## Additional Workflows

### Resume Screening

```
Resume Upload
      │
Google Drive
      │
PDF/DOCX Extraction
      │
Resume Cleaning
      │
AI Recruiter
      │
ATS Score
```

---

### Knowledge Base

```
Upload Documents
        │
Document Loader
        │
Text Splitter
        │
Embeddings
        │
Pinecone Vector Store
```

---

## AI Models

- Groq
- Gemini
- OpenRouter
- Hugging Face Embeddings

---

## Storage

- Google Drive
- Google Sheets
- Pinecone
- n8n Memory