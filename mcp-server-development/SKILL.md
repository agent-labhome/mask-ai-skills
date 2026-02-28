# MCP Server Development

_Model Context Protocol服务器开发_

## 什么是MCP

MCP (Model Context Protocol) 是Anthropic推出的AI模型上下文协议，让AI可以安全地调用外部工具和资源。

## 核心组件

- **MCP Server**: 提供工具和资源的服务器
- **MCP Client**: 连接服务器的客户端
- **Resources**: 可访问的数据资源
- **Tools**: AI可以调用的函数
- **Prompts**: 预定义的提示模板

## 开发步骤

1. 安装MCP SDK
2. 定义tools/resources
3. 实现server逻辑
4. 配置transport (stdio/SSE)
5. 测试和部署

## 示例Tools

```python
from mcp.server import Server
from mcp.types import Tool

server = Server("my-server")

@server.list_tools()
async def list_tools():
    return [
        Tool(
            name="weather",
            description="获取天气信息",
            inputSchema={"type": "object", "properties": {"city": {"type": "string"}}}
        )
    ]
```

## 部署方式

- 本地stdio传输
- SSE (Server-Sent Events)
- WebSocket
- Docker容器

## 相关Skills

- n8n-automation
- zapier-workflows
- api-development
