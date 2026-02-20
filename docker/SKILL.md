-e # Docker

{"id":"a6426dfa-2ab7-4922-96f6-def67d073974","object":"chat.completion","created":1771559296,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Docker SKILL.md

## Core Commands
- `docker run <image>` - Run container from image
- `docker build -t <name> .` - Build image from Dockerfile
- `docker ps` - List running containers
- `docker ps -a` - List all containers
- `docker images` - List images
- `docker stop <container>` - Stop container
- `docker rm <container>` - Remove container
- `docker rmi <image>` - Remove image

## Essential Concepts
- **Image**: Read-only template with instructions
- **Container**: Running instance of an image
- **Dockerfile**: Recipe for building images
- **Volume**: Persistent data storage
- **Network**: Communication between containers

## Quick Workflow
1. Write Dockerfile
2. Build: `docker build -t myapp .`
3. Run: `docker run -p 8080:80 myapp`
4"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":15,"completion_tokens":200,"total_tokens":215,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":15},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
