---
name: twitter-thread-writer
description: Twitter/X线程写作助手 - 生成病毒式传播的推特线程
auto-activate: true
version: 1.0.0
author: Mask
price: $19
categories:
  - 社交媒体
  - 内容创作
  - 个人品牌
platforms:
  - Twitter/X
---

# Twitter线程写作助手

## 功能

生成引人入胜的Twitter线程，帮助创作者、企业家、品牌快速涨粉。

## 使用场景

### 1. 知识分享线程
- 教程系列
- 行业洞察
- 学习笔记

### 2. 产品发布
- 功能介绍
- 上线预告
- 用户案例

### 3. 个人品牌
- 成长故事
- 经验总结
- 观点输出

## 参数

| 参数 | 类型 | 必填 | 说明 |
|------|------|------|------|
| topic | string | 是 | 线程主题 |
| type | string | 是 | 类型 (knowledge/product/story/opinion) |
| tweets | number | 否 | 推文数量 默认5 |
| tone | string | 否 | 语气 (专业/活泼/幽默/温暖) |

## 示例

**输入:**
```json
{
  "topic": "5个提高效率的AI工具",
  "type": "knowledge",
  "tweets": 5,
  "tone": "专业"
}
```

## 价格

- 个人版: $19
- 专业版: $49 (无限生成)
