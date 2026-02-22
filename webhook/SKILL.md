# Webhook

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Purpose
Handle incoming webhook requests from external services and process them according to configured rules.

## Core Capabilities
- **Receive & Validate**: Accept HTTP POST requests with JSON payloads
- **Security**: Verify signatures, tokens, or other authentication methods
- **Routing**: Route webhooks to appropriate handlers based on source or content
- **Transform**: Convert payload formats between different services
- **Retry Logic**: Handle failed deliveries with exponential backoff
- **Logging**: Track all incoming requests and processing results
- **Response**: Return appropriate HTTP status codes (200, 400, 401, 500, etc.)

## Common Use Cases
- GitHub/GitLab repository events (pushes, pull requests, issues)
- Payment gateway notifications (Stripe, PayPal)
- Third-party service updates (Slack, Discord, Twilio)
- IoT device data ingestion
- Form submission processing
- API synchronization triggers

## Configuration Parameters"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":15,"completion_tokens":200,"total_tokens":215,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":15},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache

## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /webhook
- Webhook
