-e {"id":"3e863d2f-39b3-49a5-a6a5-4c3fe0c8f0c9","object":"chat.completion","created":1771636394,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL: API Development

## Metadata
- **Category**: Backend Development / Software Engineering
- **Experience Level**: Intermediate to Advanced
- **Related Skills**: System Design, Database Management, Security, Testing, DevOps
- **Tools**: Postman, Swagger/OpenAPI, cURL, API Gateways
- **Common Languages**: Python (FastAPI, Django), JavaScript/TypeScript (Node.js, Express), Java (Spring Boot), Go, Ruby (Rails)

## Core Competencies

### 1. API Design Principles
- **RESTful Architecture**: Resource-based design, proper HTTP methods, statelessness
- **GraphQL**: Schema design, queries/mutations, resolver implementation
- **gRPC**: Protocol buffers, streaming, bidirectional communication
- **WebSocket**: Real-time bidirectional communication
- **API Versioning Strategies**: URL path, headers, media type, semantic versioning
- **Idempotency**: Ensuring repeated requests produce same effect
- **Pagination & Filtering**: Cursor-based vs offset pagination, query parameter design

### 2. Implementation Patterns
```python
# Example: FastAPI endpoint with validation
from fastapi import FastAPI, HTTPException, Query
from pydantic import BaseModel
from typing import Optional, List

app = FastAPI()

class Item(BaseModel):
    name: str
    price: float
    tags: List[str] = []

@app"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":20,"completion_tokens":300,"total_tokens":320,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":20},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
