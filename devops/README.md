# DevOps Automations

This folder contains **developer-focused and infrastructure-level automations** that handle scraping, domain checks, and instant landing-page generation.  
Each workflow is designed to replace repetitive technical work with **autonomous AI-powered agents**.

---

## 🕵️‍♂️ AI Agent Web-Scraping Swarm  
**File:** `AI Agent Web Scrapping.json`  

**Screenshots:**  
![AI Agent Scrapper](./Screenshots/AI%20Agent%20Scrapper.png)  
![AI Agent Scrapper - 2](./Screenshots/AI%20Agent%20Scrapper%20-%202.png)

**What it does (short):**  
- Input: *“roofing contractors in Dallas, TX, US”*.  
- GPT-4.1-mini decides which data sources to use: Google Maps, Yellow-Pages, Apollo, Instagram, TikTok.  
- Each bot scrapes business data (name, phone, email, socials).  
- Aggregates everything into **one clean Google Sheet**.  
- Removes duplicates → no manual copy-paste needed.  

---

## 🌐 Domain Name Availability Checker  
**File:** `Domain Name Availability Checker.json`  

**Screenshot:**  
![Domain Name Availability Checker](./Screenshots/Domain%20Name%20Availibility%20Checker.png)

**What it does (short):**  
- Takes a Google Sheet of domain names (e.g. `.ai`, `.com`).  
- Calls Domainr API to check availability.  
- Returns: *Active / Inactive / Taken*.  
- Writes results back to the same sheet.  
- Notifies on Slack when finished.  
- Uses rate-limiting to avoid API blocks.  

---

## 📍 Google Maps → Email Hunter  
**File:** `Google Map Email Scrapper.json`  

**Screenshots:**  
![Google Maps Email Scrapper](./Screenshots/Google%20Map%20-%20Email%20Scrapper.png)  
![Google Maps Email Scrapper - 2](./Screenshots/Google%20Maps%20Email%20Scrapper%20-%202.png)

**What it does (short):**  
- Input: list of Google Maps queries (e.g. “Hollywood dentist”).  
- Scrapes Maps results → extracts websites.  
- Visits each website → regex scrapes all e-mails.  
- Cleans + deduplicates junk addresses.  
- Appends verified e-mails into Google Sheets.  
- Fully automated local lead generation.  

---

## 🚀 Landing-Page Generator Webhook  
**File:** `Web Developer Agent for Landing Page Creation- HTML:CSS:JS .json`  

**Screenshot:**  
![Web Developer Agent](./Screenshots/Web%20Developer.png)

**What it does (short):**  
- Input: Business details (name, industry, brand colors, tone, URL).  
- GPT-5 agent generates:  
  - Conversion-optimized copy.  
  - Responsive HTML + inline CSS/JS.  
- Returns a **ready-to-use landing page file**.  
- Supports iterative “tweakPrompt” requests to edit code automatically.  
- Versions are saved + shared via Google Drive links.  

---

## Best Practices
- Always scrub scraped e-mails for GDPR/consent before campaigns.  
- Use proxy rotation or Bright Data for heavy scraping.  
- Keep separate Google Sheets for raw vs. cleaned leads.  
