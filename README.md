## 📧 AI Gmail Email Classifier (n8n Workflow)

This project automates email organization using AI. It connects to Gmail, analyzes incoming emails using a Large Language Model (LLM), and automatically assigns labels.

---

## 🚀 Features

* Real-time email classification
* AI-powered labeling
* Supports 8+ categories:

  * Academics
  * Faculty
  * Announcements
  * Events
  * Placements
  * Administrative
  * Urgent
  * Automated
* Fully automated workflow using n8n

---

## 🛠 Tech Stack

* n8n (Workflow Automation)
* Gmail API
* Groq API (Qwen 3 32B)
* AI Text Classification

---

## ⚡ How It Works

1. Gmail trigger monitors inbox
2. Extracts subject, sender, snippet
3. Sends to LLM for classification
4. Applies corresponding Gmail label

---

## 🧩 Architecture

Gmail → n8n → AI Model → Label Routing → Gmail Labels

---

## 📁 Project Structure

```
.
├── workflow.json
├── README.md
├── architecture.png
└── screenshots/
```

---

## 🚀 Setup Instructions

### 1. Install n8n

```
npm install n8n -g
```

### 2. Import Workflow

* Open n8n
* Click "Import"
* Upload workflow.json

### 3. Connect Credentials

* Gmail OAuth2
* Groq API key

### 4. Create Labels in Gmail

Create:
Academics, Faculty, Announcements, Events, Placements, Administrative, Urgent, Automated

### 5. Run Workflow

Activate → Emails auto-labeled

---

## 📊 Example

Input:
Subject: Hackathon Registration

Output:
→ Label: Events

---

## 🚀 Future Improvements

* Multi-label classification
* Email priority scoring
* Slack notifications
* Dashboard

---

## 👨‍💻 Author

Rohan Dindokar
