# n8n-ai-workflows

Production-ready n8n workflow templates with AI integrations. Import any workflow in seconds and adapt to your use case.

## Workflows

### Lead Qualification Bot
Receives a lead from any source (Typeform, Facebook, website), uses GPT-4o to score and qualify them, then routes hot leads to a human rep via Slack/WhatsApp and cold leads to an email nurture sequence.

### WhatsApp AI Responder
Connects to WhatsApp Business via webhook, maintains conversation context in a database, responds with AI-generated messages, and escalates to a human when needed.

### Invoice Processor
Watches a Google Drive folder for new PDFs. Extracts invoice data with GPT-4o Vision. Pushes results to Google Sheets and sends a Slack notification.

### CRM Contact Sync
Syncs contacts bidirectionally between any two CRMs (HubSpot, GHL, Salesforce) using n8n's built-in nodes + custom field mapping.

### Appointment Reminder Sequence
Triggered when an appointment is booked. Sends WhatsApp reminder 24h before, 1h before, and a follow-up 1h after.

## How to Import

1. Open your n8n instance
2. Go to Workflows → Import
3. Paste the JSON from any `workflows/` file
4. Configure your credentials
5. Activate

## Requirements

- n8n v1.0+ (self-hosted or n8n Cloud)
- OpenAI API key (for AI workflows)
- Relevant credentials per workflow (WhatsApp, Google, Slack, etc.)

## Folder Structure

```
workflows/
├── lead-qualification-bot.json
├── whatsapp-ai-responder.json
├── invoice-processor.json
├── crm-contact-sync.json
└── appointment-reminder.json
docs/
├── setup-guide.md
└── credential-configuration.md
```

---
Built by **Hans Aneiva** — AI automation developer, La Paz, Bolivia.
These workflows are extracted from real client projects. haneivag@gmail.com