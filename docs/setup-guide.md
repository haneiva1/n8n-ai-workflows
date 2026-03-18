# Setup Guide

## Prerequisites

- n8n instance (v1.0+)
- OpenAI API key
- Relevant third-party credentials

## Importing a Workflow

1. Download the workflow JSON from the `workflows/` folder
2. In n8n: Workflows → Import from File (or paste JSON)
3. Configure credentials in each node
4. Test with a sample trigger
5. Activate

## Environment Variables (for self-hosted n8n)

```env
N8N_ENCRYPTION_KEY=your-key
OPENAI_API_KEY=your-openai-key
```

## Common Issues

**Webhook not receiving events**: Make sure your n8n instance is publicly accessible. Use ngrok for local testing.

**AI responses too slow**: Enable streaming in the OpenAI node settings.

**Rate limits**: Add a Wait node (1-2 seconds) between API calls in batch workflows.