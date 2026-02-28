# DeepSeek V3

_中国最强开源大模型_

## 概述

DeepSeek V3是深度求索公司推出的强大开源模型，在多项基准测试中超越Llama 3.1。

## 模型规格

- 参数: 671B (37B active)
- 上下文: 64K
- 架构: Mixture of Experts (MoE)
- 训练token: 14.8T
- 发布时间: 2024-12

## 性能

- MMLU: 88.5
- HumanEval: 92.4
- Math: 90.8
- Code: 94.7

## API使用

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-xxx",
    base_url="https://api.deepseek.com"
)

response = client.chat.completions.create(
    model="deepseek-chat",
    messages=[{"role": "user", "content": "Hello"}]
)
print(response.choices[0].message.content)
```

## 本地部署

```bash
# 使用Ollama
ollama run deepseek-v3

# 使用vLLM
vllm serve deepseekai/DeepSeek-V3
```

## 定价

- API: $0.27/1M输入, $1.10/1M输出
- 开源免费本地部署

## 相关Skills

- ollama-local
- vllm-inference
- llm-deployment
