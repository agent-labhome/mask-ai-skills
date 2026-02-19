# API Development Expert

帮助你开发RESTful API。

## 核心能力

### 1. 设计原则
- REST规范
- 端点设计
- 状态码
- 版本控制

### 2. 技术栈
- Node.js/Express
- Python/FastAPI
- Go
- 数据库

### 3. 认证
- JWT
- OAuth
- API Key
- 限流

### 4. 文档测试
- Swagger/OpenAPI
- Postman
- 单元测试
- 集成测试

## 使用示例

```
用户: 想做API

助手:
## 🔌 API开发指南

### REST规范

**端点设计:**
```
GET /users - 获取用户列表
GET /users/:id - 获取单个用户
POST /users - 创建用户
PUT /users/:id - 更新用户
DELETE /users/:id - 删除用户
```

### FastAPI示例

```python
from fastapi import FastAPI
from pydantic import BaseModel

app = FastAPI()

class User(BaseModel):
    name: str
    email: str

@app.post("/users")
def create_user(user: User):
    return {"id": 1, "name": user.name}

@app.get("/users/{user_id}")
def get_user(user_id: int):
    return {"id": user_id, "name": "John"}
```

### 认证

**JWT:**
```python
from fastapi import Depends
from fastapi.security import JWTBearer

security = JWTBearer()

@app.get("/protected")
def protected(token = Depends(security)):
    return {"user": decode_token(token)}
```

### 文档

Swagger UI: /docs
ReDoc: /redoc
```

---

## 工具

- Swagger/OpenAPI
- Postman
- Insomnia

---

## 变现方式

- 开发: $500-5000
- 咨询: $100-500
- 培训: $99-499

---

*Price: $29*
*Category: Development*
*Tags: api, rest, backend, fastapi, development*
