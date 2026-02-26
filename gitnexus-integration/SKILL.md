# Gitnexus Integration

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Profile
- **Name**: GitNexus Integration
- **Type**: AI Code Intelligence & Knowledge Graph
- **Category**: AI Development Tools
- **Target Users**: Developers, AI Agents, Technical Teams
- **Price**: $39 / $79 / $149

## Overview
GitNexus是一个零服务器的代码智能引擎，可以把任何代码仓库索引为知识图谱，让AI agent获得深度代码理解能力。

## What is GitNexus?

GitNexus = Knowledge Graph for Code
- 把代码仓库转化为交互式知识图谱
- 追踪每个依赖、调用链、函数簇、执行流程
- 通过MCP协议暴露给AI agents

## Core Features

### 1. 代码索引
```bash
# 快速索引仓库
npx gitnexus analyze

# 强制重新索引
gitnexus analyze --force

# 跳过嵌入生成（更快）
gitnexus analyze --skip-embeddings
```

### 2. MCP集成
- 自动检测编辑器并配置MCP
- 支持Claude Code、Cursor、Windsurf、OpenCode
- 7个MCP工具：
  - `list_repos` - 发现所有索引仓库
  - `query` - 混合搜索（BM25 + 语义）
  - `context` - 360度符号视图
  - `impact` - 爆炸半径分析
  - `detect_changes` - Git diff影响分析
  - `rename` - 多文件重命名
  - `cypher` - 原始图查询

### 3. Agent Skills（自动安装）
- **Exploring** - 用知识图谱探索不熟悉的代码
- **Debugging** - 通过调用链追踪bug
- **Impact Analysis** - 分析变更的影响范围
- **Refactoring** - 用依赖映射计划安全重构

### 4. Web UI
- 无需安装：https://gitnexus.vercel.app
- 可视化图谱浏览器
- AI聊天界面

## Use Cases

### 1. 开发环境增强
- 让Cursor/Claude Code理解整个代码库架构
- AI不再"盲人摸象"
- 减少因不熟悉代码导致的bug

### 2. 代码审查
- 自动分析PR的影响范围
- 识别可能受影响的功能模块
- 评估改动风险

### 3. 重构规划
- 了解依赖关系后再动手
- 避免破坏调用链
- 安全地进行大型重构

### 4. 新人 onboarding
- 快速理解代码结构
- 不需要逐个文件阅读
- 通过知识图谱探索学习

## Comparison with Similar Tools

| 工具 | 特点 |
|------|------|
| **GitNexus** | 知识图谱，追踪所有关系，MCP协议 |
| **DeepWiki** | 代码理解，文档生成 |
| **Sourcegraph** | 代码搜索，企业级 |
| **Copilot** | 代码补全，上下文有限 |

## Installation & Setup

### 安装
```bash
npm install -g gitnexus
```

### 快速开始
```bash
# 进入项目目录
cd your-project

# 索引代码库
npx gitnexus analyze

# 设置MCP（一次性）
gitnexus setup

# 或手动配置Claude Code
claude mcp add gitnexus -- npx -y gitnexus@latest mcp
```

### 手动MCP配置

**Cursor** (~/.cursor/mcp.json):
```json
{
  "mcpServers": {
    "gitnexus": {
      "command": "npx",
      "args": ["-y", "gitnexus@latest", "mcp"]
    }
  }
}
```

**OpenCode** (~/.config/opencode/config.json):
```json
{
  "mcp": {
    "gitnexus": {
      "command": "npx",
      "args": ["-y", "gitnexus@latest", "mcp"]
    }
  }
}
```

## Pricing

### 免费版
- 基本功能
- 单仓库索引
- Web UI使用

### Pro版 (TODO)
- 多仓库支持
- 高级分析功能
- 优先支持

## Advantages

✅ 100%本地运行，隐私安全
✅ 轻量级，无需服务器
✅ 增强任何AI coding工具
✅ 支持多种编辑器
✅ 知识图谱比纯描述更准确

## Action Items

### 第一步：体验
```bash
# 在一个项目中运行
npx gitnexus analyze

# 打开Web UI
open https://gitnexus.vercel.app
```

### 第二步：集成到编辑器
```bash
gitnexus setup
```

### 第三步：使用MCP工具
```bash
# 查询
query({query: "authentication"})

# 查看影响
impact({file: "src/auth.js"})

# 生成文档
generate_map({format: "mermaid"})
```

## Resources
- 官网: https://gitnexus.vercel.app
- npm: https://www.npmjs.com/package/gitnexus
- GitHub: https://github.com/abhigyanpatwari/GitNexus

## Keywords
gitnexus, knowledge graph, code intelligence, AI coding, MCP, cursor, claude code, code analysis, refactoring, developer tools


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /gitnexus-integration
- Gitnexus Integration
