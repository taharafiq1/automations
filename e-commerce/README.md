# E-Commerce Automations  

This folder contains **AI and automation workflows for online stores**.  
They cover everything from **personalized shopping experiences** to **competitor tracking** and **CRM syncing**.  

---

## 🛍️ Personal Shopper Chatbot  
**File:** `Personal Shopper Chatbot.json`  

**Screenshots:**  
![Personal Shopper Chatbot - 1](./Screenshots/Personal%20Shopper%20Chatbot-1.png)  
![Personal Shopper Chatbot - 2](./Screenshots/Personal%20Shopper%20Chatbot-2.png)  

**What it does:**  
- Chat-triggered RAG agent that classifies intent:  
  - Store info (hours, address, etc.)  
  - Product search (shoes, bags, etc.)  
- Extracts keywords, price range, SKU, category.  
- Queries WooCommerce “personal_shopper” tool for matching items.  
- Otherwise consults Qdrant knowledge base for store-related answers.  

---

## 💰 Competitor Pricing Checker  
**File:** `Competitor Pricing Checker.json`  

**Screenshot:**  
![Competitor Price Checking](./Screenshots/Competitor%20Price%20Checking.png)  

**What it does:**  
- Polls competitor pricing URLs from Google Sheets.  
- Uses Airtop browser automation to scrape plan names & prices.  
- Compares against last-seen version stored in the sheet.  
- On any price change → updates the sheet + posts Slack alert with summary.  

---

## 🎯 Buyer Persona Research  
**File:** `Buyer Persona Research.json`  

**Screenshot:**  
![Buyer Persona Research](./Screenshots/Buyer%20Persona%20Research.png)  

**What it does:**  
- Public n8n form collects: *product name + number of personas*.  
- AI agent generates concise, research-backed buyer personas.  
- Appends results into Google Sheets.  
- Sends formatted HTML persona report via e-mail.  

---

## 🎨 Ads Brainstorm  
**File:** `Ads Brainstorm.json`  

**Screenshots:**  
![Ads Brainstorming](./Screenshots/Ads%20Brainstorming.png)  
![Ads Brainstorming - 1](./Screenshots/Ads%20Brainstorming-1.png)  

**What it does:**  
- Input: baseline ad image (plus optional notes).  
- Uploads image to Google Drive.  
- AI agent critiques ad psychology, design, and copy.  
- Second AI agent generates:  
  - Creative brief.  
  - Three Midjourney-style ad prompts aligned with brand playbook.  
- Posts results to Slack brainstorming channel.  

---

## 🔗 Add/Update Shopify Order to HubSpot  
**File:** `Add:Update Shopify Order to Hubspot.json`  

**Screenshot:**  
![Shopify Order to HubSpot](./Screenshots/Shopify%20Order%20to%20Hubspot.png)  

**What it does:**  
- Trigger: Shopify order updated.  
- Creates or updates customer as HubSpot contact.  
- Checks if order/deal already exists:  
  - If not → creates new **“Closed-Won” deal** with total & date.  
- Keeps Shopify & HubSpot perfectly in sync.  

---

## Best Practices  
- Use sandbox stores before connecting production Shopify/HubSpot accounts.  
- Keep competitor price tracking frequency reasonable (to avoid CAPTCHAs).  
- Add compliance checks when handling customer PII.  
