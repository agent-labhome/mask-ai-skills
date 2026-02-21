-e {"id":"7a889986-825a-440f-b6de-dec7b43dff36","object":"chat.completion","created":1771641135,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Prompt Engineering Guide

## Metadata
- **Domain**: Artificial Intelligence / Natural Language Processing
- **Primary Applications**: LLM interaction, AI-assisted workflows, content generation, problem-solving
- **Skill Level**: Beginner to Advanced
- **Prerequisites**: Basic understanding of AI/ML concepts, familiarity with any LLM interface
- **Related Skills**: Critical thinking, technical writing, domain expertise, iterative testing

## What is Prompt Engineering?

Prompt engineering is the practice of designing and optimizing inputs (prompts) to effectively communicate with large language models (LLMs) to achieve desired outputs. It combines art and science—understanding both how LLMs process information and how to structure requests for optimal results.

## Core Principles

### 1. **Clarity & Specificity**
- **Bad**: \"Tell me about history\"
- **Good**: \"Explain the three main causes of the Industrial Revolution in Britain between 1760-1840, focusing on technological, economic, and social factors\"

### 2. **Context Provision**
- **Bad**: \"Fix this code\"
- **Good**: \"I'm working on a Python Flask application. This route handler returns a 500 error when the user submits an empty form. Here's the current code: [code]. Please debug and suggest fixes with explanations.\"

### 3. **Structured Formatting**
- **Bad**: Unstructured paragraph
- **Good**: Use sections, bullet points, or explicit formatting instructions

## Practical Framework: The \"CRAFT\" Method

### **C**ontext
Provide background information and define the scenario.

**Example**:
```
Context: You are a senior software architect with 15 years of experience in scalable systems. I'm designing a microservices architecture for an e-commerce platform expecting 10,000 concurrent users.
```

### **R**ole
Assign a specific persona to the AI.

**Example**:
```
Role: Act as a professional copywriter specializing in B2B"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":22,"completion_tokens":400,"total_tokens":422,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":22},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
