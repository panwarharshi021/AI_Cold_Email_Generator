# AI Cold Email Generator

Automatically generates personalized cold emails for new leads added to a Google Sheet. When a new row is added, the workflow sends the lead's details to an AI model, generates a tailored cold email, and writes it back into the sheet — ready to send.

## How it works

1. **Google Sheets Trigger** — Watches for new rows added to a connected sheet
2. **HTTP Request** — Sends the lead's data to an AI model (via Groq API) to generate a personalized cold email
3. **Edit Fields** — Formats the AI-generated email content
4. **Update row in sheet** — Writes the generated email back into the corresponding row in Google Sheets

## Why it matters

Writing personalized cold emails for every lead is time-consuming. This automation handles it instantly — as soon as a lead is added, a ready-to-send email is generated and saved, so sales teams can move faster without sacrificing personalization.

## Built with

- [n8n](https://n8n.io) — workflow automation
- Google Sheets
- Groq API (AI text generation)

## Setup

1. Clone this repo
2. Import the workflow JSON into your n8n instance
3. Connect your Google Sheets account
4. Add your Groq API key in n8n's Credentials manager (Settings → Credentials)
5. Activate the workflow

## License

MIT
