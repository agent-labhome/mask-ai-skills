-e # Azure

{"id":"45ce3512-57ae-4af0-a413-2def25c6e96e","object":"chat.completion","created":1771547754,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Azure SKILL.md

## Core Concepts
- **Compute**: VMs, App Services, Functions, Containers (AKS)
- **Storage**: Blob, Disk, File, Queue, Table
- **Networking**: VNet, Load Balancer, VPN Gateway, DNS
- **Identity**: Azure AD, RBAC, Managed Identities

## Key Services
- **Infrastructure**: ARM templates, Azure CLI, PowerShell
- **Databases**: SQL Database, Cosmos DB, MySQL/PostgreSQL
- **Security**: Key Vault, Security Center, Sentinel
- **Monitoring**: Monitor, Application Insights, Log Analytics

## Essential Commands
```bash
az login
az group create --name <name> --location <region>
az deployment group create --template-file template.json
```

## Quick Tips
- Use Resource Groups for organization
- Enable Cost Management early
- Implement tagging strategy
