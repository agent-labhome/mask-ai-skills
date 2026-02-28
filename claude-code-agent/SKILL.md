# Claude Code Agent

_AI驱动的自动化编程助手_

## 概述

Claude Code是Anthropic推出的AI编程代理，可以自主执行复杂编程任务。

## 核心能力

- 代码生成和补全
- 项目架构设计
- Bug修复
- 测试编写
- 文档生成
- Git操作自动化

## 安装

```bash
npm install -g @anthropic-ai/claude-code
claude configure
```

## 使用方式

```bash
# 交互式
claude

# 指定任务
claude --task "修复登录bug"

# 读取文件
claude --file src/auth.py
```

## 配置

创建 `~/.claude/settings.json`:

```json
{
  "model": "claude-sonnet-4-20250514",
  "maxTokens": 4000,
  "tools": ["Read", "Write", "Bash", "grep", "glob"]
}
```

## 工作流

1. 分析任务需求
2. 制定执行计划
3. 执行代码操作
4. 运行测试验证
5. 提交更改

## 最佳实践

- 明确任务边界
- 审查自动生成的代码
- 保持版本控制
- 分阶段执行复杂任务

## 相关Skills

- ai-agent-developer
- github-actions
- git-workflow
