# AI Email Classifier & Auto-Reply — n8n Workflow

An AI-powered email automation workflow that automatically classifies incoming Gmail emails and generates professional replies using LLaMA 3.3 via Groq API.

## What It Does

- Monitors Gmail inbox every minute for new emails
- Classifies emails into two categories using Google Gemini AI:
  - **Internship** — job offers, interview invitations, hiring, recruitment
  - **Freelance** — client inquiries, project requests, Fiverr orders, AI/ML service requests
- Automatically generates a professional reply for each category using Groq (LLaMA 3.3-70b)

## Tech Stack

- **n8n** — Workflow automation platform
- **Google Gemini** — Email classification (Text Classifier)
- **Groq API (LLaMA 3.3-70b-versatile)** — AI reply generation
- **Gmail API** — Email trigger via OAuth2

## Workflow Structure
Gmail Trigger → Text Classifier (Gemini)
├── Internship → Groq API → Professional Reply
└── Freelance  → Groq API → Professional Reply

## Setup Instructions

1. Import `email-automation-workflow.json` into your n8n instance
2. Add your credentials:
   - Gmail OAuth2
   - Groq API Key — [console.groq.com](https://console.groq.com)
   - Google Gemini API Key — [aistudio.google.com](https://aistudio.google.com)
3. Activate the workflow

## Author

**Muhammad Shahan Butt** — AI/ML Engineer  
[LinkedIn](https://linkedin.com/in/shahan-butt-aiengineer) | [Portfolio](https://shahanbutt07.github.io/portfolio.me) | [GitHub](https://github.com/Shahanbutt07)
