# 📧 AI-Powered Gmail Classification Workflow

This automation flow monitors incoming Gmail messages, uses AI to analyze their content and context, and assigns smart labels for improved organization and prioritization.

---
## n8n Workflow:
!(img)[Screenshot 2025-08-15 201950.png]
---

## ⚙️ How It Works

### 1. Gmail Monitoring (Trigger)
- Continuously watches your Gmail inbox
- Polls for new emails every minute
- Captures all new messages automatically
- Runs the workflow for each incoming email

### 2. Email Content Extraction
- Retrieves complete message details:
  - Full body and headers
  - Sender and recipient info
  - Subject line and metadata
  - Existing Gmail labels/categories
  - Threading information for replies/forwards

### 3. Email History Analysis
- AI checks prior interactions:
  - Searches for past messages from the same sender
  - Looks for outbound replies in the sent folder
  - Detects first-time contacts (cold emails)
  - Analyzes the conversation thread for context

### 4. Intelligent Classification
- Uses **Claude Sonnet 4** for deep email analysis
- Considers historical context and message intent
- Detects urgency and action requirements
- Differentiates automated vs. human-sent emails

### 5. Smart Label Assignment
- Applies relevant Gmail labels automatically:
  - **To Respond** – Needs action or reply
  - **FYI** – Informational, no action needed
  - **Notification** – Service or policy updates
  - **Marketing** – Promotional/sales content
  - **Meeting Update** – Calendar changes/invites
  - **Comment** – Feedback on documents/tasks

### 6. Structured Processing
- Ensures reliable categorization:
  - Uses structured output parsing
  - Returns Gmail Label ID for direct integration
  - Applies labels automatically to emails
  - Maintains consistent classification accuracy

---

## 🛠 Tools & Technologies
- **n8n** – Workflow automation platform  
- **Gmail API** – Email monitoring & label management  
- **Anthropic Claude** – Advanced content analysis  
- **Gmail Tools** – Email search & history checks  
- **Structured Output Parser** – Consistent AI responses  

---

## 📦 Key Features
- Real-time monitoring & classification
- Context-aware analysis using past email history
- Cold vs. warm contact detection
- Multiple organization categories
- Automated Gmail label application
- Detection of automated emails via header analysis
- Thread-aware conversation tracking

---

## 🚀 Ideal For
- Executives handling high email volumes
- Sales teams prioritizing prospect responses
- Customer support managing inquiries
- Marketing teams filtering promotions
- Anyone seeking automated inbox organization
- Teams needing consistent email prioritization
