# ActivePieces MCP工作流自动化

## 描述

ActivePieces - 开源AI工作流自动化平台，400+ MCP服务器集成。适用于：(1) 无代码自动化 (2) AI工作流构建 (3) MCP集成 (4) 企业流程自动化 (5) 定时任务

## 指令

### 1. 平台概览
ActivePieces特点：
- **开源免费**: 自托管或云端使用
- **可视化编辑器**: 拖拽式流程设计
- **MCP集成**: 400+预建连接器
- **AI原生**: 内置AI动作和条件
- **实时监控**: 执行日志和告警

### 2. 快速开始
```bash
# Docker自托管
git clone https://github.com/activepieces/activepieces
cd activepieces
docker compose up -d

# 访问 http://localhost:8080
```

### 3. 核心概念
- **Pieces**: 可重用的动作模块
- **Flows**: 自动化工作流
- **Triggers**: 触发条件（定时/webhook/事件）
- **Actions**: 执行的操作
- **Branches**: 条件分支

### 4. MCP服务器集成
常用MCP集成：
- **AI服务**: OpenAI, Anthropic, Google AI
- **数据库**: PostgreSQL, MySQL, MongoDB
- **通讯**: Slack, Discord, Telegram, Email
- **云存储**: AWS S3, Google Drive
- **CRM**: HubSpot, Salesforce

### 5. AI工作流示例
```yaml
# AI内容审核流程
trigger:
  type: webhook
  
steps:
  - piece: slack
    action: new_message
    
  - piece: openai
    action: chat
    input:
      model: gpt-4
      message: "审查以下内容: {{steps.slack.message}}"
      
  - piece: conditional
    condition: "{{steps.openai.toxic}}" == true
    
  - piece: slack
    action: send_message
    if: condition_met
```

## 最佳实践

1. **模块化设计**: 复用常用流程片段
2. **错误处理**: 添加异常分支
3. **监控告警**: 设置关键节点通知
4. **版本控制**: 定期备份流程配置

## 相关工具

- n8n
- Zapier
- Make (Integromat)
- Power Automate
