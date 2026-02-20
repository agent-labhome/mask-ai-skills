-e # Kubernetes

{"id":"407f79db-ed58-4472-b5b7-1327fd2f8525","object":"chat.completion","created":1771559301,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Kubernetes SKILL.md

## Core Concepts
- **Cluster**: Set of nodes running containerized applications
- **Pod**: Smallest deployable unit (one or more containers)
- **Deployment**: Declarative way to manage Pods and ReplicaSets
- **Service**: Network abstraction for accessing Pods
- **Namespace**: Virtual cluster within a physical cluster

## Essential Commands
```bash
kubectl get pods
kubectl apply -f manifest.yaml
kubectl describe pod <name>
kubectl logs <pod-name>
kubectl exec -it <pod> -- /bin/bash
kubectl port-forward <pod> 8080:80
```

## Common Patterns
- Use Deployments for stateless applications
- Use StatefulSets for stateful applications
- Use ConfigMaps/Secrets for configuration
- Use Ingress for HTTP routing
- Use PersistentVolumes for storage
