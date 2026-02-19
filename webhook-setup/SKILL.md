-e # Webhook Setup

{"id":"35c766cb-cdae-45e4-82aa-17cdd74e32c1","object":"chat.completion","created":1771512499,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Webhook Setup

## Overview
Webhooks enable real-time notifications from external services to your application.

## Quick Setup

### 1. Generate Endpoint
Create a secure, unique URL in your app:
```
POST /api/webhooks/{service-name}
```

### 2. Configure Security
- Add signature verification (HMAC)
- Implement request validation
- Set up IP whitelisting if available

### 3. Handle Events
- Parse incoming payload
- Validate required data
- Process asynchronously
- Return `200 OK` immediately

### 4. Monitoring
