# n8n-automation-projects

This repository contains a collection of **Automation Workflows and AI Agents built with n8n**.  

## 📌 Projects Included

### 1️⃣ AI Agent Email Assistant

**Description**  
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


