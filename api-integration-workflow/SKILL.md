# API Integration Workflow Skill

## Description
Build automated workflows that connect different APIs and services - from simple triggers to complex multi-step integrations.

## Use Cases
- Connect CRM to marketing tools
- Automate data synchronization between apps
- Create custom notifications and alerts
- Build no-code automation pipelines
- Sync inventory across platforms

## Instructions

### Popular Integration Platforms

**No-Code (Easy):**
| Platform | Best For | Price |
|----------|----------|-------|
| Zapier | General automation | Free-$600/mo |
| Make (Integromat) | Complex workflows | Free-$300/mo |
| Pabbly | Budget-friendly | Free-$99/mo |
| n8n | Self-hosted/advanced | Free (self-hosted) |

**Code-Based (Advanced):**
| Tool | Use Case |
|------|----------|
| Node.js + Express | Custom APIs |
| Python + FastAPI | Data processing |
| Serverless (Vercel/Netlify) | Event-driven |

### Building Your First Integration

**1. Define the Flow:**
```
Trigger (A) → Action (B) → Transform (C) → Action (D)
```

**2. Choose Your Components:**

**Trigger Options:**
- Webhook (real-time)
- Schedule (cron)
- App event (new lead, purchase, etc.)

**Action Options:**
- Create record
- Update data
- Send notification
- Call another API

**3. Example: New Shopify Order → QuickBooks Invoice**

```
Step 1: Shopify Webhook
- Event: Order created
- Data: Customer, items, total

Step 2: Transform
- Map to QuickBooks format
- Calculate taxes

Step 3: QuickBooks API
- Create invoice
- Send to customer
```

### API Connection Templates

**REST API Call:**
```javascript
async function callAPI(url, method, data, headers) {
  const response = await fetch(url, {
    method: method,
    headers: {
      'Content-Type': 'application/json',
      ...headers
    },
    body: JSON.stringify(data)
  });
  return response.json();
}
```

**Webhook Handler:**
```javascript
app.post('/webhook', async (req, res) => {
  const { action, data } = req.body;
  
  switch(action) {
    case 'new_lead':
      await addToCRM(data);
      break;
    case 'order_placed':
      await processOrder(data);
      break;
  }
  
  res.status(200).send('OK');
});
```

### Authentication Methods

| Method | Use Case | Setup |
|--------|----------|-------|
| API Key | Simple APIs | Header: `X-API-Key: key` |
| Bearer Token | OAuth2 | Header: `Authorization: Bearer token` |
| Basic Auth | Legacy APIs | Header: `Authorization: Basic base64(user:pass)` |
| OAuth 2.0 | User-authorized apps | Redirect flow + token refresh |

### Troubleshooting

**Common Issues:**
1. **401 Errors** - Token expired → Implement refresh
2. **Rate Limiting** - Too many requests → Add delay/queue
3. **Data Format** - Mismatch → Use transformer
4. **Timeout** - Long operations → Async/queue

## Advanced Patterns

**Retry Logic:**
```javascript
async function withRetry(fn, maxAttempts = 3) {
  for (let i = 0; i < maxAttempts; i++) {
    try {
      return await fn();
    } catch (err) {
      if (i === maxAttempts - 1) throw err;
      await delay(1000 * Math.pow(2, i));
    }
  }
}
```

**Queue-Based Processing:**
- Use Redis/Bull for background jobs
- Prevent API rate limiting
- Handle failures gracefully
