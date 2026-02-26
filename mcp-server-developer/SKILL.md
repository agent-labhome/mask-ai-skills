# Skill: mcp-server-developer

## 触发词
- MCP服务器开发
- MCP集成
- Model Context Protocol

## 功能描述
帮助开发者创建MCP (Model Context Protocol) 服务器，实现：
- 自定义工具暴露给AI Agent
- 私有API集成
- 数据库操作封装
- 文件系统交互
- 第三方服务连接

## 使用场景
1. 将私有API暴露给AI助手
2. 创建自定义数据库工具
3. 构建企业内部Agent
4. 集成遗留系统

## 价格
$49/$99/$199

## MCP架构

### 核心概念
- **Server**: 提供工具和资源的MCP服务
- **Client**: 连接服务器的AI应用
- **Tools**: 可调用的函数
- **Resources**: 可读取的数据
- **Prompts**: 预定义提示模板

### 开发步骤
1. 定义工具schema
2. 实现工具handler
3. 添加资源端点
4. 配置认证和限流
5. 部署到VPS/Docker

### Python示例
```python
from mcp.server import Server
from mcp.types import Tool

server = Server("my-server")

@server.list_tools()
async def list_tools():
    return [Tool(
        name="query_db",
        description="Query database",
        inputSchema={"type": "object", "properties": {"sql": {"type": "string"}}}
    )]
```

### 托管方案
- Railway: 免费$5/月
- Render: 免费
- VPS: $5/月 DigitalOcean
