# 📧 n8n Email Automation (Gmail + Google Sheets)

This repository contains a cleaned n8n workflow for automating follow-up emails.  
It integrates Gmail and Google Sheets to send targeted messages, track opens and clicks, and update contact records.

## 🚀 How It Works
- Fetch contact data from Google Sheets.
- Apply conditional logic to decide whether to send Email #1 or Email #2.
- Send emails via Gmail.
- Track email opens and link clicks via a webhook.
- Update Google Sheets with tracking data.

## 🛠 Setup
1. Run your n8n environment (local or cloud).
2. Add Gmail and Google Sheets credentials in n8n UI.
3. Import `workflows/myWorkflow.json` via **Import from File**.
4. Copy `.env.example` to `.env` and fill in:
   - `GOOGLE_SHEET_ID` – your Google Sheets document ID
   - `N8N_HOST` – your n8n host URL
   - `N8N_WEBHOOK_ID` – your webhook node ID

> Note: This workflow uses placeholders for sensitive values. Replace them with your own before running.

## 🧩 Requirements
- n8n v1.70 or later
- Gmail and Google Sheets nodes enabled

## ✉️ Features
- Conditional automated follow-up emails
- Email open & click tracking
- Data updates back into Google Sheets

## ⚠ Security
- No API keys or credentials are included in this repository.
- Create credentials directly in your n8n environment.
- Use webhook URLs only in secure environments.
