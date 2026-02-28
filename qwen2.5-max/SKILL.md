# Qwen 2.5 Max

_阿里最强闭源大模型_

## 概述

Qwen 2.5 Max是阿里巴巴推出的旗舰级AI模型，在中文理解和生成方面处于领先地位。

## 模型系列

- Qwen 2.5 (开源)
- Qwen 2.5 Plus
- **Qwen 2.5 Max** (最强闭源)
- Qwen 2.5 Turbo (快速版)

## 核心能力

- 超强中文理解
- 代码编写调试
- 数学推理
- 创意写作
- 多轮对话
- Agent能力

## API调用

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-xxx",
    base_url="https://dashscope.aliyuncs.com/compatible-mode/v1"
)

response = client.chat.completions.create(
    model="qwen-max",
    messages=[{"role": "user", "content": "写一首关于AI的诗"}]
)
```

## 适用场景

- 中文内容创作
- 商业文案
- 技术文档
- 智能客服
- 教育辅导

## 定价

- qwen-max: ¥20/1M输入, ¥60/1M输出
- qwen-plus: ¥4/1M输入, ¥12/1M输出
- qwen-turbo: ¥1/1M输入, ¥3/1M输出

## 相关Skills

- qwen-local-deployment
- alibaba-cloud-ai
- chinese-llm
