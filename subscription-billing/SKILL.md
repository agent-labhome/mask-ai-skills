-e {"id":"fc82f88e-e30c-4f8e-8e90-09271b9c8801","object":"chat.completion","created":1771671536,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL: Subscription Billing

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata
- **Domain**: E-commerce / SaaS / Digital Services
- **Complexity**: Intermediate to Advanced
- **Key Concepts**: Recurring revenue, billing cycles, dunning, proration, compliance
- **Common Systems**: Stripe, Recurly, Chargebee, Zuora, PayPal Subscriptions
- **Related Skills**: Payment Processing, Revenue Recognition, Customer Retention

## Practical Guide

### 1. Core Subscription Models
**Fixed Plans**
- Tiered pricing (Basic, Pro, Enterprise)
- Per-seat/user pricing
- Usage-based tiers with hard limits

**Usage-Based**
- Pay-as-you-go (per API call, GB stored, etc.)
- Hybrid (base fee + overage charges)
- Tiered usage (different rates at different volumes)

**Freemium**
- Free tier with paid upgrades
- Time-limited trials
- Feature-gated plans

### 2. Billing Cycle Fundamentals
**Cycle Types**
- Monthly (most common)
- Annual (often with discount)
- Quarterly/Semi-annual
- Custom durations

**Key Dates**
- **Anniversary date**: When subscription renews
- **Invoice date**: When bill is generated (often 1-30 days before renewal)
- **Due date**: When payment is required
- **Grace period**: Buffer before service suspension

### 3. Implementation Checklist

**Pre-Launch**
- [ ] Define clear pricing pages and terms
- [ ] Set up tax calculation (VAT, GST, sales tax)
- [ ] Configure webhooks for billing events
- [ ] Implement dunning management (failed payments)
- [ ] Create subscription lifecycle emails
- [ ] Plan proration logic for upgrades/downgrades

**Customer Experience**
- [ ] Self-service portal for plan changes
- [ ] Transparent billing history
- [ ] Easy cancellation flow (consider regulations)
- [ ] Pro-rated refund policy
- [ ] Clear communication on renewal dates

**Operations**
- [ ] Automated dunning sequence (3+ attempts)
- [ ] Failed payment recovery workflow
- [ ] Churn analysis reporting
- [ ] Revenue recognition setup
- [ ] Invoice customization (branding, localization)

### 4. Common Scenarios & Solutions

**Upgrades/Downgrades**
```javascript
// Example proration logic
if (upgradeMidCycle) {
 "},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":20,"completion_tokens":500,"total_tokens":520,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":20},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /subscription-billing
- Subscription Billing
