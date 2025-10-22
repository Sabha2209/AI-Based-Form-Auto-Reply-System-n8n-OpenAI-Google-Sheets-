# 🤖 AI-Powered Form Submission Auto-Responder (n8n + OpenAI + Google Sheets)

An intelligent automation workflow built using **n8n** and **OpenAI GPT**, designed to:
✅ Collect form submissions  
✅ Auto-generate personalized email responses using AI  
✅ Store user data into a Google Sheet for tracking  

---

## 🎯 Purpose
This project aims to automate customer form handling processes by instantly replying to user submissions using AI, and safely logging the data in a central storage (Google Sheets). It saves manual time and provides a professional response experience for users.

---

## ✳️ Real-World Use Cases
| Use Case                 | Description |
|--------------------------|------------|
| 📩 Contact Us Form       | Auto-thanks user & replies with basic info |
| 🎓 Student Query Form    | Sends instant informative reply |
| 💼 Job Application Form  | Sends acknowledgment & next steps |
| 📢 Event Registration    | Confirms registration via email |
| 📊 Lead Generation       | Logs leads & sends quick response |

---

## 🚀 Features
✅ Form submission trigger (n8n Form / Google Form via webhook)  
✅ AI-generated personalized reply using OpenAI GPT  
✅ Automatic email response to the user  
✅ Saves name, email, message & timestamp into Google Sheets  
✅ Works for multiple users dynamically (unlimited submissions)

---

## 🧠 Workflow Overview

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| n8n | Workflow automation |
| OpenAI GPT | Generates email responses |
| Gmail / Outlook | Sends dynamic emails |
| Google Sheets | Saves submission data |

---

## 📍Step-by-Step Workflow

### ✅ 1. Form Trigger
- Use `Form Trigger` in n8n OR connect a Google Form via webhook.
- Example fields: `name`, `email`, `message`.

### ✅ 2. OpenAI AI Response
Prompt example:


### ✅ 3. Auto Email Node
- Use Gmail/Outlook node  
- To: `{{$json["email"]}}`  
- Subject: `Thank you, {{$json["name"]}}!`  
- Message: Response from AI node  

### ✅ 4. Save to Google Sheets
- Create columns: Name | Email | Message | Date  
- Append row with submission data.

---

## 📂 Example Google Sheet Format

| Name | Email | Message | AI Response | Date |
|------|-------|---------|-------------|------|

---

## 📦 Future Enhancements
✅ Add WhatsApp/Twilio SMS reply  
✅ Use classification to route to different teams  
✅ Add sentiment analysis  
✅ Add CRM integration (Notion/HubSpot)

---

## 📜 License
This project is open-source under the MIT License.

---

## ✨ Author
Created by _Your Name (Sabapathi R)_ as part of AI workflow automation projects using n8n.
