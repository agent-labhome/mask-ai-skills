-e {"id":"1857dcad-b64c-43d1-a48c-3334b83ca717","object":"chat.completion","created":1771597010,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"```markdown
---
name: Account Management
description: Handles user account operations including creation, updates, verification, and closure.
triggers:
  - \"create account\"
  - \"update profile\"
  - \"verify account\"
  - \"close account\"
  - \"reset password\"
  - \"account settings\"
---

# Account Management

## Capabilities
- Create new user accounts with required information
- Update user profile details (email, preferences, contact info)
- Process account verification requests
- Handle account closure/deletion procedures
- Manage password resets and security settings
- Modify notification and privacy preferences

## Requirements
- User authentication for sensitive operations
- Data validation for all inputs
- Confirmation steps for irreversible actions
- Compliance with data protection regulations
- Audit logging for security-critical changes

## Output
- Success/error messages with clear next steps
- Confirmation emails for critical changes
- Updated account records
- Security event notifications
```"},"logprobs":null,"finish_reason":"stop"}],"usage":{"prompt_tokens":26,"completion_tokens":200,"total_tokens":226,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":26},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
