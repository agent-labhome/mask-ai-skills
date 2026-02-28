# Claude Code Dev

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## 描述

Anthropic Claude Code (claude.ai/code) 本地AI编程助手开发指南。适用于：(1) Claude Code安装与配置 (2) 本地开发环境集成 (3) 项目初始化 (4) Agent模式开发 (5) 自定义Rules配置

## 指令

当用户需要使用Claude Code进行本地开发时：

### 1. 安装与配置
- Claude Code可通过官网下载或包管理器安装
- 配置CLAUDE.md项目规则文件
- 设置工作目录和项目上下文

### 2. 项目初始化
- 使用 `claude` 命令启动交互式会话
- 配置 .claude/settings.json 全局设置
- 初始化项目特定的 Rules

### 3. Agent开发模式
- 理解Claude Code的Agent能力（文件操作、代码修改、终端命令）
- 使用 `/compact` 压缩上下文
- 使用 `/web` 进行网络搜索
- 配置允许的目录和命令

### 4. 高级用法
- 创建项目级CLAUDE.md规则
- 集成到现有开发工作流
- 自定义快捷方式和命令
- 与VS Code/ JetBrains集成

### 5. 故障排除
- 权限问题排查
- 网络连接问题
- 上下文窗口管理

## 示例

```
# 初始化新项目
claude init my-project

# 在当前目录启动
claude

# 使用特定规则
claude --rules .claude/project-rules.md
```

## 相关工具

- VS Code
- JetBrains IDEs
- Terminal
- Git


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /claude-code-dev
- Claude Code Dev
