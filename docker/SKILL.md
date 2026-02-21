# Docker: Containerization Platform

## Metadata
- **Category**: DevOps / Containerization
- **Complexity**: Intermediate
- **Prerequisites**: Basic Linux/CLI, understanding of virtualization concepts
- **Related Skills**: Kubernetes, CI/CD, Cloud Platforms, Infrastructure as Code
- **Market Demand**: High (Essential for modern DevOps roles)

## Overview
Docker is a platform for developing, shipping, and running applications in containers. Containers package an application with all its dependencies, ensuring consistency across environments.

## Core Concepts

### 1. **Container Fundamentals**
- **Images**: Read-only templates with instructions for creating containers
- **Containers**: Runnable instances of images
- **Dockerfile**: Text document with commands to assemble an image
- **Registry**: Repository for Docker images (Docker Hub, private registries)

### 2. **Key Components**
- Docker Engine (daemon + CLI)
- Docker Compose (multi-container applications)
- Docker Swarm (native clustering)
- Docker Hub (public registry)

## Practical Skills

### Basic Operations
```bash
# Image management
docker pull nginx:latest
docker images
docker rmi <image_id>

# Container lifecycle
docker run -d -p 8080:80 --name web nginx
docker ps -a
docker stop/start/restart <container>
docker rm <container>

# Interactive container
docker run -it ubuntu bash
"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":17,"completion_tokens":300,"total_tokens":317,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":17},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
