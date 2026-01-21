# n8n-automation-projects

This repository contains a collection of **Automation Workflows and AI Agents built with n8n**.  

## 📌 Projects Included

### 1️⃣ AI Agent Email Assistant
An AI-powered email assistant that sends personalized emails to customers based on natural language chat requests.

Instead of manually searching for contact details and writing emails, the AI agent understands the user request, finds the correct customer, and sends the email automatically.

### 🔄 Workflow Logic

1. A chat message is received (example: “Send an email to Maria B”)
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



