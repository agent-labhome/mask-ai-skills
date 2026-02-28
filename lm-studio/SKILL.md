# LM Studio

_桌面端大模型运行工具_

## 概述

LM Studio是一个强大的桌面应用，让你在Mac/Windows上轻松运行本地大模型。

## 核心功能

- 一键下载模型
- GUI界面操作
- 本地API服务器
- Chat UI交互
- GPU加速支持
- 模型管理

## 支持平台

- macOS (Apple Silicon + Intel)
- Windows (x64)
- Linux (AppImage)

## 安装

从 https://lmstudio.ai 下载安装包

## 使用流程

1. 打开LM Studio
2. 在模型浏览器搜索下载模型
3. 选择模型并加载
4. 开始对话或启动API

## API使用

```bash
# 启动本地API
curl http://localhost:1234/v1/chat/completions \
  -H "Content-Type: application/json" \
  -d '{
    "model": "llama-3.1-8b-instruct",
    "messages": [{"role": "user", "content": "Hi"}]
  }'
```

## 推荐配置

| 场景 | 模型 | VRAM |
|------|------|------|
| 聊天 | Llama 3.1 8B | 6GB |
| 编程 | CodeLlama 7B | 8GB |
| 总结 | Mistral 7B | 6GB |

## 与Ollama对比

| 特性 | LM Studio | Ollama |
|------|-----------|--------|
| UI | 丰富 | 命令行 |
| 模型格式 | GGUF | 原创 |
| API兼容 | OpenAI | 自有 |
| 调参 | 详细 | 基础 |

## 相关Skills

- ollama-local
- gguf-models
- local-ai-deployment
