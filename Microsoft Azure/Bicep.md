---
created: 2023-11-21T12:19:04Z
updated: 2024-12-10T08:34:58Z
tags:
  - azure
  - declarative
  - DSL
  - IaC
  - idempotent
  - template
documentation:
  - https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/
---
- A declarative [[DSL]] for defining and deploying [[Azure]] infrastructure
- Bicep files can be deployed with [[Azure CLI]] or [[Azure PowerShell]] by including the template file:
	- Azure CLI: `--template-file <bicep-file>`
	- Azure PowerShell: `-Templatefile`