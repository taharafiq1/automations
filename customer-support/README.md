# Customer Support Automations

This folder contains workflows that automate **customer communication across email, voice, and WhatsApp**.  
They’re designed to reduce support load, provide instant AI-driven replies, and escalate only when necessary.

---

## 📧 AI Based Customer Support Agent  
**File:** `AI Based Customer Support Agent.json`  

**Screenshot:**  
![Customer Support Agent](./Screenshots/Customer%20Support%20Agent.png)

**What it does (short):**  
- Watches a Gmail inbox for incoming messages.  
- Uses GPT-4.1-nano to classify and answer directly from a Google Docs knowledge base.  
- If the query can be answered → auto-replies with the extracted answer.  
- If not → forwards the mail to a human support team inbox.  

---

## 📞 AI Based Voice Call Agent  
**File:** `AI Based Voice Call Agent.json`  

**Screenshot:**  
![Voice Call Agent](./Screenshots/Voice%20Call%20Agent.png)

**What it does (short):**  
- Takes a plain-English request like *“Call barber John at … for a 6 pm haircut”*.  
- Converts it into a structured Vapi call payload (number, context, opening line).  
- Launches the outbound call, waits for it to finish.  
- Returns the **call transcript** for logging and follow-up.  

---

## 📱 WhatsApp Advanced AI Agent  
**File:** `Whatsapp advanced AI Agent.json`  

**Screenshot:**  
![WhatsApp Advanced AI Agent](./Screenshots/WhatsApp%20Advanced%20AI%20Agent.png)

**What it does (short):**  
- Listens to incoming WhatsApp messages (text, voice, images, PDFs).  
- Responds with:  
  - **Text →** GPT-4o-mini replies instantly.  
  - **Voice →** transcribes and returns AI-generated speech.  
  - **Images →** AI generates a description.  
  - **PDFs →** AI summarizes and sends key points.  
- Keeps a **short-term 10-turn memory** to maintain context.  

---

## Best Practices
- Keep logs of AI responses for review/QA.  
- Always mask/remove sensitive customer data before training.  
- Add human-in-the-loop escalation paths for high-risk cases.  
