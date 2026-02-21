# SKILL: Kubernetes

## Metadata
- **Category**: DevOps & Infrastructure
- **Subcategory**: Container Orchestration
- **Prerequisites**: 
  - Container fundamentals (Docker)
  - Basic Linux command line
  - YAML syntax
  - Networking concepts
- **Experience Level**: Intermediate to Advanced
- **Common Roles**: DevOps Engineer, SRE, Platform Engineer, Cloud Engineer

## Overview
Kubernetes is an open-source container orchestration platform that automates deployment, scaling, and management of containerized applications. Originally developed by Google, it's now maintained by the Cloud Native Computing Foundation (CNCF).

## Core Concepts

### 1. **Cluster Architecture**
- **Control Plane**: Manages the cluster (API Server, etcd, Scheduler, Controller Manager)
- **Nodes**: Worker machines that run containers (kubelet, kube-proxy, container runtime)
- **Pods**: Smallest deployable units (one or more containers sharing resources)
- **Services**: Stable network endpoints for pods
- **Ingress**: Manages external HTTP/S traffic to services

### 2. **Key Objects**
```yaml
# Example Pod definition
apiVersion: v1
kind: Pod
metadata:
  name: myapp-pod
spec:
  containers:
  - name: myapp-container
    image: nginx:latest
    ports:
    - containerPort: 80
```

###"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":17,"completion_tokens":300,"total_tokens":317,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":17},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
