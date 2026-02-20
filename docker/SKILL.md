-e # Docker

{"id":"a39c0d0c-af4c-4d5e-be4f-42996aa5b461","object":"chat.completion","created":1771547735,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Docker SKILL.md

## Core Commands
- `docker run <image>` – Run container from image
- `docker build -t <name> .` – Build image from Dockerfile
- `docker ps` – List running containers
- `docker ps -a` – List all containers
- `docker images` – List images
- `docker stop <container>` – Stop container
- `docker rm <container>` – Remove container
- `docker rmi <image>` – Remove image

## Key Concepts
- **Image** – Read-only template with instructions
- **Container** – Running instance of an image
- **Dockerfile** – Recipe for building images
- **Volume** – Persistent data storage
- **Network** – Communication between containers

## Common Workflow
1. Create Dockerfile
2. Build image: `docker build -t myapp .`
3. Run container: `docker run -p 808"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":15,"completion_tokens":200,"total_tokens":215,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":15},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
