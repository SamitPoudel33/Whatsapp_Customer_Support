# 🤖 WhatsApp AI Agent — n8n Workflow

This repository contains an **n8n AI Agent** that connects **WhatsApp**, **Google Gemini**, and **Google Sheets** to automate intelligent WhatsApp replies using AI.

---

## 🧩 Overview

The workflow listens for incoming WhatsApp messages, sends them to the **Google Gemini Chat Model**, retrieves or stores related data in **Google Sheets**, and replies intelligently via WhatsApp.

### 🧱 Components
- **WhatsApp Trigger** — Starts the workflow when a new message is received.  
- **AI Agent** — The main orchestrator (LangChain integration).  
- **Google Gemini Chat Model** — Handles message understanding and response generation.  
- **Simple Memory** — Keeps conversational context across messages.  
- **Google Sheets** — Fetches or logs relevant data for the AI Agent.  
- **Send Message** — Sends the AI’s response back to the WhatsApp user.  

---

## 📁 Folder Structure
```
n8n-whatsapp-ai-agent/
├── agents/
│   └── whatsapp.json       # Exported workflow file from n8n
├── screenshots/
│   └── workflow-preview.png
├── README.md
├── .gitignore
└── LICENSE
```

---

## 🚀 How to Use

1. Open your **n8n instance**.  
2. Click **Import Workflow**.  
3. Upload the file `agents/whatsapp.json`.  
4. Set up these credentials inside n8n:
   - WhatsApp API (Trigger + Send)
   - Google Gemini (PaLM) API
   - Google Sheets OAuth2
5. Click **Activate Workflow** and start chatting on WhatsApp!

---

## ⚙️ Requirements
- n8n version **1.0+**
- WhatsApp Business API credentials  
- Google Gemini (PaLM) API key  
- Google Sheets access  
- Stable Internet connection

---

## 🔒 Security
🚫 **Do not upload credentials** to GitHub.  
Before sharing your workflow publicly:
- Remove or anonymize any `credential` blocks from the JSON.
- Use `.gitignore` to exclude sensitive files.

---

## 📜 License
Released under the [MIT License](LICENSE).
