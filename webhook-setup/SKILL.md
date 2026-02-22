## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

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

## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /webhook-setup
- Webhook Setup
