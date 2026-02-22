# Chatbot Development

帮助你开发AI聊天机器人。

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## 核心能力

### 1. 平台选择
- ChatGPT API
- Claude API
- 开源模型
- 自托管

### 2. 开发框架
- LangChain
- LlamaIndex
- AutoGen
- Custom

### 3. 对话设计
- Prompt工程
- 上下文管理
- 记忆系统
- 工具集成

### 4. 部署运维
- API服务
- 前端集成
- 监控
- 成本优化

## 使用示例

```
用户: 想做AI客服

助手:
## 🤖 聊天机器人指南

### 技术栈

**API方案:**
- GPT-4 API
- FastAPI后端
- Streamlit前端

### 代码示例

```python
from openai import OpenAI
from fastapi import FastAPI

app = FastAPI()
client = OpenAI()

@app.post("/chat")
async def chat(message: str):
    response = client.chat.completions.create(
        model="gpt-4",
        messages=[{"role": "user", "content": message}]
    )
    return response.choices[0].message.content
```

### Prompt设计

**系统提示词:**
```
你是一个专业的客服助手。
- 礼貌友好
- 简洁明了
- 解决用户问题
```

### 成本优化

- 使用GPT-3.5处理简单问题
- 只对复杂问题用GPT-4
- 设置最大token限制
```

---

## 工具

- OpenAI API
- Anthropic API
- FastAPI
- Streamlit

---

## 变现方式

- 开发: $500-5000
- 部署: $200-2000
- 培训: $99-499

---

*Price: $39*
*Category: Development*
*Tags: chatbot, ai, openai, gpt, langchain*


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /chatbot-development
- Chatbot Development
