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


