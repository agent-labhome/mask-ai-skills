-e {"id":"efabff86-f7a9-40c4-a9f6-7843df9ecd10","object":"chat.completion","created":1771671600,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL: API Integration

## Metadata
- **Category**: Development/Backend
- **Complexity**: Intermediate
- **Prerequisites**: 
  - Basic programming knowledge
  - Understanding of HTTP protocols
  - Familiarity with JSON/XML formats
- **Time to Learn**: 2-4 weeks
- **Key Tools**: Postman, cURL, programming language HTTP libraries
- **Related Skills**: Authentication, Data Serialization, Error Handling

## Practical Guide

### 1. Understanding APIs
**What is an API?**
- Application Programming Interface (API) - a set of rules allowing software applications to communicate
- Typically uses HTTP/HTTPS protocols
- Common formats: REST, GraphQL, SOAP

**Key Concepts:**
- **Endpoints**: URLs where API resources are located
- **Methods**: GET, POST, PUT, DELETE, PATCH
- **Status Codes**: 200 (OK), 201 (Created), 400 (Bad Request), 401 (Unauthorized), 404 (Not Found), 500 (Server Error)
- **Headers**: Metadata about the request/response
- **Body**: Data being sent/received (JSON, XML, form-data)

### 2. Getting Started

**Tools Setup:**
```bash
# Install common tools
# Postman (GUI) - Download from postman.com
# cURL (Command line) - Usually pre-installed
# Choose a programming language library:
# Python: requests, httpx
# JavaScript: axios, fetch API
# Java: OkHttp, Retrofit
```

**First API Call (cURL Example):**
```bash
# Basic GET request
curl https://api.example.com/data

# With headers
curl -H \"Content-Type: application/json\" \
     -H \"Authorization: Bearer YOUR_TOKEN\" \
     https://api.example.com/data
```

### 3. Authentication Methods

**Common Authentication Types:**

1. **API Keys**:
```python
import requests

headers = {
    \"X-API-Key\": \"your-api-key-here\"
}
response = requests.get(\"https://api.example.com/data\", headers=headers)
```

2. **Bearer Tokens (OAuth 2.0)**:
```python
headers = {
    \"Authorization\": \"Bearer YOUR_ACCESS_TOKEN\"
}
```

3. **Basic Auth**:
```python
from"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":19,"completion_tokens":500,"total_tokens":519,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":19},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
