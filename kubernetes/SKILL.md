-e # Kubernetes

{"id":"9aa0e970-0bad-4d0a-bb9f-653a5275fe2e","object":"chat.completion","created":1771547739,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Kubernetes SKILL.md

## Core Concepts
- **Pods**: Smallest deployable units (one or more containers)
- **Services**: Network endpoints for pods
- **Deployments**: Declarative updates for pods and ReplicaSets
- **ConfigMaps & Secrets**: Configuration and sensitive data management
- **Namespaces**: Virtual clusters within a physical cluster

## Essential Commands
```bash
kubectl get pods,svc,deploy
kubectl apply -f manifest.yaml
kubectl describe resource/name
kubectl logs pod-name
kubectl exec -it pod-name -- /bin/bash
kubectl port-forward svc/name 8080:80
```

## Common Patterns
- Use Deployments over bare Pods
- Liveness/readiness probes for health checks
- Resource requests/limits for stability
- Horizontal Pod Autoscaling (HPA) for scaling
- Ingress"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":15,"completion_tokens":200,"total_tokens":215,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":15},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
