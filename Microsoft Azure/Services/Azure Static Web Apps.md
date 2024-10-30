---
aliases:
  - SWA
documentation:
  - https://learn.microsoft.com/en-us/azure/static-web-apps/
training:
  - https://learn.microsoft.com/en-us/training/paths/azure-static-web-apps/
---
# Description
- Static assets ([[HTML]], [[JavaScript]], [[CSS]], images) are served from globally distributed servers
- [[API]] endpoints are hosted [[Serverless Computing|serverlessly]] with [[Azure Functions]]
- Can connect to [[GitHub]] and [[Azure Repos]]
- Utilizes workflows in [[GitHub Actions]] or [[Azure Pipelines]]
	- When there are changes, these workflows build and deploy the app and API
- Has free SSL certificates which are automatically renewed
- Offers preview [[URL]]s for [[Pull Request|pull requests]]
- [[Fallback routes]] are handled in `staticwebapp.config.json`