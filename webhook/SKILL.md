-e # Webhook

{"id":"e9dd48c4-564e-41b7-b393-696c9ea4e5ff","object":"chat.completion","created":1771555739,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Webhook SKILL

## Purpose
Handle incoming webhook requests and process payload data.

## Core Commands
- `webhook receive` - Process incoming webhook data
- `webhook list` - Show recent webhook events
- `webhook test` - Send test webhook payload

## Key Features
- Parse JSON/XML payloads
- Validate signatures
- Route to appropriate handlers
- Log incoming requests
- Retry failed deliveries

## Usage Examples
```bash
# Process incoming webhook
webhook receive --source=stripe --event=payment.succeeded

# View recent webhooks
webhook list --last=10
