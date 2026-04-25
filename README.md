# n8n-automation-projects

This repository contains a collection of **Automation Workflows and AI Agents built with n8n**.  

## 📌 Projects Included

### 1️⃣ AI Agent Email Assistant
An AI-powered email assistant that sends personalized emails to customers based on natural language chat requests.

Instead of manually searching for contact details and writing emails, the AI agent understands the user request, finds the correct customer, and sends the email automatically.

### 🔄 Workflow Logic

1. A chat message is received
2. The AI Agent analyzes the message:
   - Identifies the customer name
   - Extracts the email content
3. The workflow searches a Google Sheets customer database
4. The customer’s email address is retrieved
5. A personalized email is composed and sent via Gmail

### 🛠 Tools & Technologies

- **n8n** – Workflow automation
- **OpenAI** – AI Agent reasoning & language understanding
- **Google Sheets** – Customer database
- **Gmail API** – Email delivery

____________________________________________________________________________________________________________________________

### 2️⃣ Motivational Quote Generator
 
An automated workflow that generates a motivational quote every day at 7 AM using AI and sends it by email to a list of recipients.

The workflow runs automatically every day at 7 AM, delivering daily motivation without any manual action.

### 🔄 Workflow Logic

1. Schedule trigger runs daily at 7 AM
2. OpenAI generates a motivational quote
3. Google Sheets retrieves recipient email addresses
4. Gmail sends the quote to all recipients

### 🛠 Tools & Technologies
- n8n
- OpenAI (GPT-4 Mini)
- Google Sheets
- Gmail API

____________________________________________________________________________________________________________________________

### 3️⃣ AI Document Summarizer

An AI-powered workflow that automatically summarizes uploaded PDF documents and stores the results for future reference.

The workflow starts when a user submits a form with a PDF file. The document text is extracted, summarized using AI, enriched with contextual knowledge, and saved to Google Sheets.

### 🔄 Workflow Logic

1. Workflow is triggered on form submission
2. User uploads a PDF document
3. Text is extracted from the file
4. AI model generates a clear and concise summary
5. Wikipedia tool is used for additional context when needed
6. Title, summary, and date are saved to Google Sheets

### 🛠 Tools & Technologies

- n8n
- OpenAI (Message Model)
- Wikipedia Tool
- Google Forms (file upload)
- Google Sheets (Append row in sheet)

### 📄 Stored Data (Google Sheets)

| Title | Summary | Date Added |
|------|--------|-----------|

____________________________________________________________________________________________________________________________

### 4️⃣ Data Backup System (Form → OneDrive → Google Sheets)

An automated data backup workflow that stores job application data securely by saving uploaded resumes to OneDrive and logging applicant information in Google Sheets.

This workflow ensures that applicant files and metadata are safely backed up and easily accessible.

### 🔄 Workflow Logic

1. Workflow is triggered on form submission
2. Applicant submits personal information and resume
3. Resume file is uploaded to OneDrive
4. Applicant data and file URL are appended to Google Sheets
   
### 🛠 Tools & Technologies

- n8n
- Google Forms (file upload)
- OneDrive
- Google Sheets

### 📄 Stored Data (Google Sheets)

| Full Name | Email | Position Applied For | File URL |
|---------|-------|----------------------|----------|

____________________________________________________________________________________________________________________________

### 5️⃣ LinkedIn Post Generator

**Description**  
An AI-powered workflow that generates professional, research-based LinkedIn posts.

Users submit a form with a post topic and target audience. The system researches the topic, writes a high-quality LinkedIn post, and prepares the content for publishing and email delivery.

### 🔄 Workflow Logic

1. Workflow starts on form submission
2. AI agent researches the topic using Tavily (real-time search)
3. AI agent writes a professional LinkedIn post tailored to the audience
4. Post is published on LinkedIn and sent a confirmation email
   
### 🛠 Tools & Technologies

- n8n
- OpenAI 
- Tavily Search API
- Gmail
- LinkedIn API

____________________________________________________________________________________________________________________________

### 6️⃣ Gmail Inbox Classifier & Auto-Responder (AI-Powered)
An AI-powered Gmail automation system that automatically classifies incoming emails and sends responses based on their intent.
The workflow analyze email content, classifies messages into preddfined categories, applies Gmail labels, and sends tailored replies without manual intervention.

### 🔄 Workflow Logic
1. Gmail trigger listens for new incoming messages.
2. AI extracts key information from the email.
3. Data is cleaned and normalized.
4. AI classifier categorizes the email:
   - Service Requests
   - Payments
   - Consultations Requests.
   - Others.
5. Gmail labels are applied automatically.
6. Predefined responses are sent based on the category.
   
### 🛠 Tools & Technologies
- n8n
- OpenAI
- Gmail API
______________________________________________________________________________________________________________________

### 7️⃣ AI-Powered Client Onboarding System

A fully automated, production-ready client onboarding system that triggers the moment a new client submits a form — instantly sending a personalized AI-generated welcome email, creating a CRM contact in HubSpot with an AI-written profile summary, scheduling a welcome call in Google Calendar, notifying the internal team on Slack, logging everything to Google Sheets, and automatically sending a follow-up email 2 days later.
Every action runs in parallel. Every failure is handled gracefully. Every execution is logged with real statuses — not hardcoded values.

### 🔄 Workflow Logic

1. Workflow is triggered when a new client submits a form
2. Client data is cleaned and structured
3. AI generates a structured client summary
4. Client data is stored in Google Sheets
5. Contact is created in HubSpot (CRM)

**Parallel onboarding actions:**

6. AI generates a personalized welcome email → sent via Gmail  
7. A welcome call is automatically scheduled via Google Calendar  
8. Internal team is notified via Slack  

**Follow-up automation:**

9. System waits for 2 days  
10. AI generates a follow-up email  
11. Follow-up email is sent automatically  
12. Execution is logged in Google Sheets  

### 🛠 Tools & Technologies

- n8n
- OpenAI (GPT-4 Mini – summary, emails, follow-ups)
- Google Sheets (data storage & logging)
- Gmail API (email communication)
- Google Calendar (meeting scheduling)
- Slack (team notifications)
- HubSpot CRM (contact management)
