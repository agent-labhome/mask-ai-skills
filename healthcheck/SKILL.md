---
name: healthcheck
description: Host security hardening and risk assessment for OpenClaw deployments
auto-activate: true
version: 1.0.0
author: Mask
price: $39
categories:
  - Security
  - DevOps
  - Infrastructure
platforms:
  - Linux
  - Server
---

# HealthCheck Security Assistant

## 功能

主机安全加固和风险评估工具。

## 使用场景

### 1. 安全审计

**输入:** 服务器信息

**输出:**
- 漏洞列表
- 风险等级
- 修复建议

### 2. 防火墙配置

**输入:** 服务器类型

**输出:**
- iptables规则
- SSH加固
- 端口管理

### 3. 风险评估

**输入:** 当前配置

**输出:**
- 风险分数
- 薄弱环节
- 改进建议

### 4. 版本检查

**输入:** 组件列表

**输出:**
- 可用更新
- 安全补丁
- 建议版本

## 参数

| 参数 | 类型 | 必填 | 说明 |
|------|------|------|------|
| task | string | 是 | 任务类型 |
| os | string | 是 | 操作系统 |
| components | string | 否 | 组件列表 |

## 示例

### 安全审计

**输入:**
```json
{
  "task": "审计",
  "os": "Ubuntu 22.04"
}
```

**输出:**
```
🔒 安全审计报告

📊 风险评分: 75/100

⚠️ 发现问题:
1. SSH root登录 enabled (高风险)
2. 防火墙未配置 (高风险)
3. 系统未更新 (中风险)

✅ 正常:
- 用户权限合理
- 密码策略已启用

💡 修复建议:
1. 禁用root SSH登录
2. 配置UFW防火墙
3. 执行系统更新
```

## 价格

- 基础版: $39/月
- 专业版: $89/月 (自动修复)
- 企业版: $249/月 (定制+监控)

## 更新日志

### v1.0.0 (2026-02-19)
- 初始版本
- 安全审计/防火墙/风险评估/版本检查
