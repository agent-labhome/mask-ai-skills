# SKILL.md: LLM Fine-tuning

## Metadata
- **Skill Level**: Intermediate to Advanced
- **Prerequisites**: 
  - Python programming
  - Basic ML/DL concepts
  - Familiarity with PyTorch/Hugging Face
  - Access to GPU resources
- **Time to Proficiency**: 2-4 weeks
- **Related Skills**: Prompt Engineering, RAG, Model Evaluation, ML Ops
- **Tools**: Hugging Face Transformers, PyTorch, LoRA/QLoRA, Weights & Biases, Axolotl

## Overview
LLM fine-tuning adapts pre-trained language models to specific tasks, domains, or behaviors. Unlike prompt engineering which works with frozen models, fine-tuning actually modifies model weights to improve performance on target tasks.

## Core Concepts

### Types of Fine-tuning
1. **Full Fine-tuning**: Updates all model parameters (resource-intensive)
2. **Parameter-Efficient Fine-tuning (PEFT)**: 
   - LoRA (Low-Rank Adaptation): Adds trainable rank decomposition matrices
   - QLoRA: Quantized LoRA for memory efficiency
   - Prefix Tuning: Learns continuous prompt embeddings
   - Adapter Layers: Adds small trainable modules between layers

### Data Formats
- **Instruction Tuning**: (Instruction, Input, Output) triples
- **Chat Format**: Multi-turn conversations with roles
- **Completion Format**: Simple (prompt, completion) pairs

## Practical Guide

### Step 1: Problem Definition & Data Preparation

**Define your objective:**
```python
# Example: Customer support chatbot
objective = {
    \"task\": \"multi-turn customer support\",
    \"domain\": \"e-commerce tech support\",
    \"desired_behaviors\": [
        \"empathetic tone\",
        \"accurate troubleshooting\",
        \"clear step-by-step guidance\",
        \"brand-appropriate language\"
    ]
}
"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":24,"completion_tokens":400,"total_tokens":424,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":24},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
