# vLLM推理服务

_生产级大模型推理框架_

## 概述

vLLM是NVIDIA开发的高性能大模型推理服务框架，支持PagedAttention和持续批处理。

## 核心特性

- PagedAttention (减少显存)
- 持续批处理 (高吞吐)
- 张量并行 (多GPU)
- OpenAI兼容API
- 动态批处理
- FP8量化支持

## 安装

```bash
# CUDA 12.1+
pip install vllm

# 从源码
git clone https://github.com/vllm-project/vllm.git
cd vllm
pip install -e .
```

## 快速启动

```bash
# 命令行推理
vllm serve meta-llama/Llama-3.1-8B-Instruct

# OpenAI API
curl http://localhost:8000/v1/chat/completions \
  -H "Content-Type: application/json" \
  -d '{
    "model": "meta-llama/Llama-3.1-8B-Instruct",
    "messages": [{"role": "user", "content": "Hello"}]
  }'
```

## Docker部署

```bash
docker run --gpus all \
  -v ~/.cache/huggingface:/root/.cache/huggingface \
  -p 8000:8000 \
  vllm/vllm-openai \
  --model meta-llama/Llama-3.1-8B-Instruct
```

## 性能对比

| 框架 | Toke/s | 显存效率 |
|------|--------|----------|
| HF | 50 | 1x |
| vLLM | 200+ | 2x |

## 支持模型

- Llama 3.1
- Mistral
- Qwen 2.5
- DeepSeek V3
- Gemma 2
- 以及100+开源模型

## 生产部署

```bash
# 多GPU
vllm serve meta-llama/Llama-3.1-70B-Instruct \
  --tensor-parallel-size 4

# 高并发
vllm serve meta-llama/Llama-3.1-8B \
  --max-num-seqs 256 \
  --enforce-eager
```

## 相关Skills

- ollama-local
- lm-studio
- k8s-llm-serving
