# job-cover-later-assistant
# AI Job Application Assistant

An AI-powered SaaS application that automatically generates personalized job application documents using Google Gemini and n8n.

---

## Live Demo

https://coverlatter.lovable.app/

---

## Features

- Upload Resume (PDF)
- Paste Job Description
- Extract Resume Text Automatically
- AI-Powered Cover Letter Generation
- ATS-Friendly Resume Summary
- HTML Template Generation
- PDF Generation
- Merge Multiple PDFs
- Automatic Email Delivery
- End-to-End Workflow Automation

---

## Tech Stack

- n8n
- Google Gemini API
- JavaScript
- HTML
- CSS
- Docker
- Gotenberg
- Gmail
- Webhooks

---

## Workflow

User Form

↓

Webhook

↓

Extract Resume PDF

↓

Google Gemini

↓

Generate Cover Letter

↓

Generate Resume Summary

↓

Split AI Output

↓

Generate HTML Templates

↓

Convert HTML to PDF

↓

Merge PDFs

↓

Send Email

---

## Project Architecture

```
Lovable Form
      │
      ▼
Webhook
      │
      ▼
Extract From PDF
      │
      ▼
Google Gemini AI
      │
      ▼
Code Node
      ├────────► Cover Letter HTML
      │                 │
      │                 ▼
      │          Cover Letter PDF
      │
      └────────► Resume Summary HTML
                        │
                        ▼
                Resume Summary PDF
                        │
                        ▼
                  Merge PDFs
                        │
                        ▼
                    Gmail
```

---

## Screenshots

Add your workflow screenshots here.

---

## Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

### Run n8n

```bash
docker run -it --rm \
-p 5678:5678 \
-v n8n_data:/home/node/.n8n \
n8nio/n8n
```

### Run Gotenberg

```bash
docker run -d --name gotenberg -p 3000:3000 gotenberg/gotenberg:8
```

---

## Environment Variables

Create the following credentials inside n8n:

- Google Gemini API
- Gmail OAuth2
- Gotenberg
- Webhook URL

---

## Future Improvements

- User Authentication
- Application History
- Dashboard
- Multiple Resume Support
- ATS Score
- Job Match Percentage
- Interview Suggestions
- Resume Optimizer

---

## Live Demo

https://coverlatter.lovable.app/

---

## GitHub Repository

Add your repository link here.

---

