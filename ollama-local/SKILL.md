# Ollama本地大模型

_在本地运行开源大模型_

## 概述

Ollama让你在本地设备上运行开源大模型，无需GPU也可以运行小型模型。

## 支持模型

- Llama 3.1 (8B, 70B)
- Mistral (7B)
- Phi 3 (4B)
- DeepSeek Coder (6.7B)
- Qwen 2.5 (0.5B-72B)
- Gemma 2 (2B, 9B)
- 以及更多...

## 安装

```bash
# macOS
brew install ollama

# Linux
curl -fsSL https://ollama.com/install.sh | sh

# Windows (WSL2)
```

## 基本使用

```bash
# 拉取模型
ollama pull llama3.1

# 运行模型
ollama run llama3.1

# 列出已安装模型
ollama list
```

## API服务

```bash
# 启动API服务
ollama serve

# 调用API
curl http://localhost:11434/api/generate -d '{
  "model": "llama3.1",
  "prompt": "Hello"
}'
```

## 硬件要求

| 模型 | RAM | GPU |
|------|-----|-----|
| 7B | 8GB | 可选 |
| 13B | 16GB | 推荐 |
| 70B | 64GB | 必须 |

## 高级功能

- 自定义模型导入
- Modelfile配置
- 多模型同时运行
- GPU加速

## 相关Skills

- lm-studio
- vllm-inference
- local-llm-deployment
