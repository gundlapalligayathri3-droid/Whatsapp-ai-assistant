# 🤖 AI-Powered WhatsApp Business Assistant with RAG

An enterprise-grade AI-powered WhatsApp chatbot built using **n8n**, **OpenAI GPT**, **MongoDB Atlas Vector Search**, and the **WhatsApp Business Cloud API**. The assistant intelligently processes text, voice notes, images, PDFs, Word documents, Excel files, and JSON files to deliver accurate, context-aware responses using **Retrieval-Augmented Generation (RAG)**.

---

## 🚀 Features

- 💬 WhatsApp Business Cloud API integration
- 🧠 Retrieval-Augmented Generation (RAG)
- 🔍 MongoDB Atlas Vector Search
- 🤖 OpenAI GPT-powered AI Agent
- 🖼️ Image understanding and OCR support
- 🎙️ Voice note transcription (Speech-to-Text)
- 📄 PDF document processing
- 📑 Word document support
- 📊 Excel file processing
- 📋 JSON parsing
- 💾 Conversation memory
- 🧭 Intelligent routing based on message type
- 🛡️ Guardrails to reduce hallucinations
- ❓ Clarification questions for ambiguous queries
- ⚠️ Graceful error handling for unsupported files and API failures

---

## 🏗️ Workflow Architecture

```text
WhatsApp Business Cloud API
            │
            ▼
     WhatsApp Trigger
            │
            ▼
     Route by Message Type
            │
 ┌──────────┼──────────┐
 │          │          │
 ▼          ▼          ▼
Text     Image      Voice
 │          │          │
 ▼          ▼          ▼
Process   OCR     Speech-to-Text
 │          │          │
 └──────────┼──────────┘
            ▼
     Convert to Text
            │
            ▼
      Prompt Mapping
            │
            ▼
        AI Agent
            │
            ▼
MongoDB Vector Search (RAG)
            │
            ▼
 Retrieve Relevant Chunks
            │
            ▼
      OpenAI GPT Model
            │
            ▼
   Generate Final Response
            │
            ▼
 Reply via WhatsApp
```

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------|
| Workflow Automation | n8n |
| LLM | OpenAI GPT |
| Vector Database | MongoDB Atlas Vector Search |
| Messaging Platform | WhatsApp Business Cloud API |
| AI Architecture | Retrieval-Augmented Generation (RAG) |
| OCR | OCR/Vision Model |
| Speech Recognition | Speech-to-Text |
| Prompt Engineering | System Prompt + Dynamic Prompt Mapping |

---

## 📂 Supported Input Types

- ✅ Text Messages
- ✅ Voice Notes
- ✅ Images
- ✅ PDF Documents
- ✅ Word Documents (.docx)
- ✅ Excel Files (.xlsx)
- ✅ JSON Files

---

## 🧠 AI Capabilities

The assistant can:

- Answer questions using uploaded business documents
- Retrieve information using semantic vector search
- Process multiple document formats
- Maintain conversational context
- Ask follow-up questions when necessary
- Detect greetings and small talk
- Handle unsupported file types gracefully
- Avoid hallucinations by relying on retrieved knowledge

---

## 📌 Example Use Cases

- Customer Support
- HR Policy Assistant
- Employee Self-Service
- Internal Knowledge Base
- Company Documentation Assistant
- FAQ Automation
- Business Process Automation

---

## 📁 Repository Structure

```
Whatsapp-ai-assistant/
│
├── README.md
├── whatsapp_ai_assistant_workflow.json
├── screenshots/
└── assets/
```

---

## ⚙️ Getting Started

### Prerequisites

- n8n
- OpenAI API Key
- MongoDB Atlas Cluster with Vector Search
- WhatsApp Business Cloud API
- Meta Developer Account

### Import Workflow

1. Download the workflow JSON.
2. Open **n8n**.
3. Select **Import from File**.
4. Choose the workflow JSON.
5. Configure your credentials:
   - OpenAI
   - MongoDB Atlas
   - WhatsApp Business Cloud API
6. Activate the workflow.

---

## 🔒 Security

Before deploying:

- Store API keys using n8n Credentials.
- Never commit secrets to GitHub.
- Use environment variables where applicable.
- Enable logging and monitoring for production.

---

## 🚀 Future Improvements

- Multi-language support
- Human handoff integration
- CRM integration
- Calendar scheduling
- Email automation
- Analytics dashboard
- Feedback collection
- Sentiment analysis

---

## 📸 Screenshots

<img width="960" height="564" alt="Screenshot 2026-07-27 222601" src="https://github.com/user-attachments/assets/68e07edd-0611-494d-b752-06267ed94a93" />




Example:

```
screenshots/
├── workflow.png
├── ai-agent.png
└── architecture.png
```

---

## 👩‍💻 Author

**Lakshmi Gayathri Gundlapalli**

B.Tech – Materials Science & Metallurgical Engineering  
IIT Hyderabad

---

## ⭐ If you found this project useful

If you like this project, consider giving it a ⭐ on GitHub!
