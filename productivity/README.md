# 🛠️ Productivity Automations  

This folder contains **AI + automation workflows** designed to save time, centralize tasks, and extract insights.  
From an all-in-one **personal assistant** to **content intelligence analyzers**, these workflows maximize efficiency.  

---

## 🤖 Ultimate Personal Assistant  
**File:** `Ultimate Personal Assistant.json`  

**Screenshots:**  
![Ultimate Personal Assistant - 5](./Screenshots/Ultimate%20Personal%20Assistant.png) 
![Ultimate Personal Assistant - 1](./Screenshots/Ultimate%20Personal%20Assistant-1.png)  
![Ultimate Personal Assistant - 2](./Screenshots/Ultimate%20Personal%20Assistant-2.png)  
![Ultimate Personal Assistant - 3](./Screenshots/Ultimate%20Personal%20Assistant-3.png)  
![Ultimate Personal Assistant - 4](./Screenshots/Ultimate%20Personal%20Assistant-4.png)  
 

**What it does:**  
- Listens to Slack messages (text, voice, or images) from **Mr. Taha**.  
- Routes input through a **humorous AI “router” agent**, which decides which sub-agent to call:  
  - Contacts  
  - Calendar  
  - Email  
  - Tasks (ClickUp)  
  - Finance  
  - Reminders  
  - Research  
  - AI-Voice Call Bot  
- Keeps **memory of past chats** for contextual awareness.  
- Turns **one Slack window** into your central productivity hub:  
  - Book haircuts.  
  - Log expenses.  
  - Send emails.  
  - Create ClickUp tasks.  
  - Place AI-voice calls.  

---

## 📰 Daily AI Newsletter  
**File:** `Daily AI Newsletter.json`  

**Screenshot:**  
![Daily AI Newsletter](./Screenshots/Daily%20AI%20Newsletter.png)  

**What it does:**  
- Runs **every morning at 11 AM**.  
- Queries **Perplexity** for the latest 48h of AI news.  
- Cross-checks headlines against a Google Sheets archive to **avoid duplicates**.  
- Sends a **colorful HTML digest of 5 fresh stories** via email.  
- Appends stories to the archive sheet for future de-duplication.  

---

## 📊 YouTube Comments Analyzer  
**File:** `Youtube Comments Analyzer.json`  

**Screenshot:**  
![YouTube Comments Analyzer](./Screenshots/Youtube%20Comments%20Analyzer%20copy.png)  

**What it does:**  
- Fetches **comments** from a YouTube video.  
- Runs **sentiment analysis** to identify trends.  
- Extracts:  
  - Strengths & weaknesses of the content.  
  - Audience pain points & questions.  
  - Recurring keywords.  
  - Topic clusters.  
  - Competitors & external references.  
- Produces a **structured insight report** for:  
  - Content improvement.  
  - Audience understanding.  
  - Competitive positioning.  

---

## ✅ Best Practices  
- For the **Personal Assistant**, use a sandbox Slack workspace before going live.  
- Respect YouTube API quotas when analyzing large comment sets.  
- Store insights and newsletters in a database or Sheets for long-term tracking.  
