# Gemini 2.0 Flash

_Google最新快速响应AI模型_

## 概述

Gemini 2.0 Flash是Google DeepMind推出的新一代快速响应模型，主打低延迟高效能。

## 核心特点

- 超快响应速度 (<1秒)
- 1M token上下文
- 原生多模态 (文本/图片/音频/视频)
- 128K输出token
- 低价格 ($0.075/1M输入)

## API使用

```python
import google.generativeai as genai

genai.configure(api_key="YOUR_API_KEY")
model = genai.GenerativeModel('gemini-2.0-flash')

response = model.generate_content("解释量子计算")
print(response.text)
```

## 适用场景

- 实时对话
- 快速摘要
- 代码生成
- 内容审核
- 低延迟应用

## 限制

- 知识截止: 2025-01
- 15 RPM (免费版)
- 100 TPM (免费版)

## 相关Skills

- google-ai-studio
- gemini-pro
- multimodal-ai
