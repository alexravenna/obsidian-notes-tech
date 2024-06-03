---
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
- A declarative [[DSL]] for defining and deploying [[Microsoft Azure/Azure]] infrastructure
- Bicep files can be deployed with [[Azure CLI]] or [[Azure PowerShell]] by including the template file:
	- Azure CLI: `--template-file <bicep-file>`
	- Azure PowerShell: `-Templatefile`