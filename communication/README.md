# Communication Automations

This folder contains workflows that improve and automate communication across platforms such as **WhatsApp** and **YouTube**. These automations save time, deliver insights, and streamline engagement with audiences.

---

## 📌 Workflows

### 1. YouTube Comments Analyzer
**File:** `Youtube Comments Analyzer.json`  
**Screenshot:**  
![YouTube Comments Analyzer](./Screenshots/Youtube%20Comments%20Analyzer.png)

**What it does:**  
- Fetches comments from any YouTube video.  
- Performs sentiment analysis to gauge audience reaction.  
- Identifies strengths & weaknesses of the content.  
- Extracts audience pain points, questions, recurring keywords and topic clusters.  
- Finds external references and competitor mentions.  

**Use case:** Content creators, social media teams, and marketing strategists who want actionable audience insights to improve content and strategy.

---

### 2. WhatsApp Advanced AI Agent
**File:** `Whatsapp advanced AI Agent.json`  
**Screenshots:**  
![WhatsApp Advanced AI Agent](./Screenshots/WhatsApp%20Advanced%20AI%20Agent.png)  
![WhatsApp Advanced AI Agent - Response](./Screenshots/WhatsApp%20Advanced%20AI%20Agent-Response.png)

**What it does:**  
- Listens to incoming WhatsApp messages (text, voice, image, PDF).  
- **Text:** Answers via GPT-4o-mini (context-aware).  
- **Voice notes:** Transcribes to text, generates reply, optionally sends TTS response.  
- **Images:** Describes image contents and extracts useful text/labels.  
- **PDFs:** Summarizes documents and returns a short summary or key points in chat.  
- Sends replies back into the same WhatsApp conversation; logs conversation data for analytics.

**Use case:** Customer support, personal assistant automation, sales follow-up, and multi-format user interactions.

---

## 🚀 Value Summary
- Faster response times and 24/7 handling of common queries.  
- Actionable audience insights from YouTube comments (content iteration + product feedback).  
- Multi-format handling (voice, image, PDF) on WhatsApp improves UX and reduces manual triage.

---

## 🛠 How to run (quick)
1. Import the `.json` into your n8n instance.  
2. Configure provider credentials (WhatsApp API/VAPI, YouTube API, OpenAI/OpenRouter).  
3. Enable the workflow and test with sample inputs.

---
