-e # Webhook

{"id":"b5198efe-852f-40b0-9125-cfad556feba2","object":"chat.completion","created":1771585013,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL: Webhook

## Purpose
Handle incoming HTTP webhook events from external services.

## Core Capabilities
- **Receive & Validate**: Accept POST requests with JSON payloads
- **Security**: Verify signatures/headers (when configured)
- **Process**: Parse payload and trigger appropriate workflows
- **Respond**: Return appropriate HTTP status codes (200, 400, etc.)

## Configuration
```yaml
webhook:
  endpoint: /webhook/{service}
  methods: [POST]
  security:
    - signature_verification
    - ip_whitelist
  timeout: 30s
```

## Common Use Cases
- Payment gateway notifications (Stripe, PayPal)
- CI/CD pipeline events (GitHub, GitLab)
