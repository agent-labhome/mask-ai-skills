---
name: task-automation
description: 任务自动化助手 - Cron Jobs、定时任务、工作流自动化
auto-activate: true
version: 1.0.0
author: Mask
price: $49
categories:
  - 自动化
  - 效率
  - 开发
platforms:
  - 通用
---

# 任务自动化助手

## 功能

帮助你设置和管理定时任务、自动化工作流。

## 使用场景

### 1. Cron任务设置

**输入:** 任务描述

**输出:**
- Cron表达式
- 执行时间说明
- 验证命令

### 2. 自动化工作流

**输入:** 工作流描述

**输出:**
- 步骤分解
- 所需工具
- 实现建议

### 3. 定时提醒

**输入:** 提醒内容 + 时间

**输出:**
- 设置命令
- 确认方式

## 参数

| 参数 | 类型 | 必填 | 说明 |
|------|------|------|------|
| task | string | 是 | 任务类型: cron/workflow/reminder |
| description | string | 是 | 任务描述 |
| schedule | string | 否 | 时间规格 |

## 示例

**输入:**
```json
{
  "task": "cron",
  "description": "每天上午9点发送天气报告",
  "schedule": "daily 9am"
}
```

**输出:**
```
⏰ Cron任务设置

表达式: 0 9 * * *
验证: crontab -l

执行命令:
curl -s "https://api.weather.com/..."
| mail -s "Daily Weather" user@example.com

💡 提示: 使用crontab -e编辑
```

## 价格

- 免费版: 基础cron表达式
- 专业版: $49/月 (复杂工作流+监控)
- 企业版: $129/月 (自定义集成)

## 更新日志

### v1.0.0 (2026-02-20)
- 初始版本
- Cron任务/工作流/提醒
