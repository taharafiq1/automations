# CRM Automations

Workflows in this folder focus on **lead generation, enrichment, and high-velocity outreach** — built to turn raw lists and form inputs into clean, personalized lead rows you can actually use for outreach.

---

## 1) Automate Hyper-Personalized Outreach at Scale  
**File:** `Automate Hyper-Personalized Outreach at Scale.json`  

**Screenshot:**  
![Automate Hyper Personalized Outreach](./Screenshots/Automate%20Hyper%20Personalized%20Outreach.png)

**What it does (short):**  
- Starts from a target list (name/company/LinkedIn URL or a search seed).  
- Scrapes LinkedIn for location, company, recent posts (via Bright Data).  
- An LLM (Claude/OpenRouter) writes a tight **4-line opener** tailored to each profile.  
- Results are appended row-by-row into Google Sheets ready for cold email or outreach sequences.

**Flow:**  
1. Read target list  
2. Scrape LinkedIn (location, company, recent post snippets)  
3. Generate 4-line opener via LLM  
4. Save: `name | company | title | linkedin_url | recent_post | opener` into Google Sheets

---

## 2) Cold Email Ice Breaker  
**File:** `Cold Email Ice Breaker.json`  

**Screenshot:**  
![Cold Email Ice Breaker](./Screenshots/Cold%20Email%20Ice%20Breaker.png)

**What it does (short):**  
- Turns a list of company websites into ready-to-send cold email elements:  
  - Catchy subject line  
  - 1–2 line opener relevant to each business  

**Flow:**  
1. Read companies list from Google Sheets  
2. Fetch each website, strip HTML  
3. LLM generates subject + opener  
4. Save results back to the same sheet

---

## 3) Automate Hyper-Personalized Outreach at Scale
**File:** `Generate & Enrich LinkedIn Leads with Apollo & LinkedIn API.json`  


**What it does (short):**  
- Input: job title, location, lead count  
- Pulls matching people from Apollo.io  
- Gets LinkedIn + verified email  
- Scrapes profile & recent posts  
- Summarizes via GPT-3.5 into 2 paragraphs  
- Saves everything row-by-row into Google Sheets

---
