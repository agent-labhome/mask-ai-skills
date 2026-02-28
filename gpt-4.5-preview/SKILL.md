# GPT-4.5 Preview

_OpenAI最新预览版模型_

## 概述

GPT-4.5是OpenAI在GPT-4o之后的下一代预览模型，主打更好的理解力和创造力。

## 发布时间

2025-02 (Preview版)

## 核心改进

- 更自然的对话
- 更好的情感理解
- 减少幻觉
- 改进的推理能力
- 更广泛的知识覆盖

## API使用

```python
from openai import OpenAI

client = OpenAI()
response = client.chat.completions.create(
    model="gpt-4.5-preview",
    messages=[{"role": "user", "content": "解释机器学习"}]
)
print(response.choices[0].message.content)
```

## 限制

- 仅Chat API可用
- 速率限制较严格
- 上下文窗口: 128K
- 输出token: 8K

## 定价

- 输入: $75/1M tokens
- 输出: $150/1M tokens

## 使用建议

1. 用于需要高理解力的复杂任务
2. 创意写作和内容创作
3. 高级对话系统
4. 不适合大批量简单任务

## 相关Skills

- openai-api
- gpt-4o
- prompt-engineering
