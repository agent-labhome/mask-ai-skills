-e # Node.js

{"id":"01ce8712-99bd-401c-8819-4d97e0016950","object":"chat.completion","created":1771559173,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Node.js SKILL.md

## Core Concepts
- **Runtime**: JavaScript runtime built on Chrome's V8 engine
- **Event Loop**: Non-blocking, asynchronous I/O model
- **Module System**: CommonJS (require/module.exports) and ES Modules

## Essential APIs
- **fs**: File system operations (sync/async)
- **http/https**: Create servers and make requests
- **path**: Cross-platform path manipulation
- **events**: Event emitter pattern
- **stream**: Handle large data efficiently

## Package Management
- **npm**: Default package manager (or use **yarn**/**pnpm**)
- **package.json**: Project manifest and dependencies
- **node_modules**: Dependency storage (exclude from version control)

## Common Patterns
- Middleware architecture (Express.js)
- Error-first callbacks
- Promises/async-await for async operations
- Environment variables (process.env)
