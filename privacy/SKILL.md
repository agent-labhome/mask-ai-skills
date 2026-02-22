# Privacy

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata
- **Category**: Security & Compliance
- **Level**: Intermediate to Advanced
- **Last Updated**: 2024
- **Related Skills**: Security, Data Protection, Compliance, Encryption, GDPR, HIPAA

## Overview
Privacy engineering is the discipline of designing, implementing, and maintaining systems that protect personal data throughout its lifecycle. It goes beyond legal compliance to embed privacy into the architecture and culture of software development.

## Core Concepts

### 1. Privacy Principles
- **Data Minimization**: Collect only what's necessary
- **Purpose Limitation**: Use data only for specified purposes
- **Storage Limitation**: Retain data only as long as needed
- **Accuracy**: Ensure data is accurate and up-to-date
- **Integrity & Confidentiality**: Protect against unauthorized processing
- **Accountability**: Demonstrate compliance with privacy principles

### 2. Privacy by Design
- **Proactive not Reactive**: Anticipate and prevent privacy issues
- **Privacy as Default**: Maximum privacy without user action
- **Privacy Embedded into Design**: Integral part of system architecture
- **Full Functionality**: Positive-sum, not zero-sum solutions
- **End-to-End Security**: Full lifecycle protection
- **Visibility & Transparency**: Keep it open and verifiable
- **Respect for User Privacy**: Keep it user-centric

## Practical Implementation

### 1. Data Classification
```yaml
# Example data classification policy
data_classes:
  public:
    description: \"Non-sensitive information\"
    examples: [\"product descriptions\", \"public blog posts\"]
    
  internal:
    description: \"Company confidential\"
    examples: [\"internal memos\", \"meeting notes\"]
    
  confidential:
    description: \"Sensitive business information\"
    examples: [\"financial projections\", \"strategic plans\"]
    
  restricted:
    description: \"Highly sensitive personal data\"
    examples: [\"SSN\", \"health records\", \"biometric data\"]
    requirements: [\"encryption\", \"access logs\", \"consent tracking\"]
```

### 2. Privacy Impact Assessments (PIA)
```python
# PIA checklist implementation
class PrivacyImpactAssessment:
    def"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":17,"completion_tokens":450,"total_tokens":467,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":17},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /privacy
- Privacy
