---
created: 2024-10-01T20:00:28Z
updated: 2024-12-10T08:34:57Z
documentation:
  - https://learn.microsoft.com/en-us/azure/developer/terraform/
---
# Description
- [[Infrastructure as Code/Terraform/Terraform|Terraform]] [[provider]] for [[Azure]] ecosystem:
	- AzureRM: for managing [[Azure Resource Manager|ARM]] resources; most user-friendly
		- uses Azure SDK for Go under the hood
	- AzureAD: for managing [[Microsoft Entra ID]] resources
	- AzureDevOps: for managing [[Azure DevOps]] resources
	- AzAPI: for managing Azure [[Resource|resources]] by using the ARM APIs directly; most up-to-date
		- uses direct [[REST]] [[API]] calls to the [[Azure Resource Manager]] REST API
	- github: for managing [[GitHub]]
	- Azure Stack: for managing  [[Azure Stack]] resources