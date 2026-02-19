-e # Webhook

{"id":"43a26230-d217-4020-91f3-eda12ffd19c8","object":"chat.completion","created":1771523333,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Webhook SKILL

## Purpose
Handle incoming webhook requests and forward them to appropriate channels.

## Commands
- `webhook create <name>` - Generate a new webhook URL
- `webhook list` - Show active webhooks
- `webhook delete <name>` - Remove a webhook
- `webhook info <name>` - Show webhook details

## Usage
1. Create a webhook to receive external data
2. Configure external services to send POST requests to your webhook URL
3. Webhook payloads are automatically forwarded to the channel where the webhook was created

## Features
- Unique URLs per webhook
- JSON payload forwarding
- Automatic channel notifications
- Simple management commands"},"logprobs":null,"finish_reason":"stop"}],"usage":{"prompt_tokens":16,"completion_tokens":153,"total_tokens":169,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":16},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
