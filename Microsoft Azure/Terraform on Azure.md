---
documentation:
  - https://learn.microsoft.com/en-us/azure/developer/terraform/
---
# Description
- [[Infrastructure as Code/Terraform/Terraform|Terraform]] [[Providers]] for [[Azure]] ecosystem:
	- AzureRM: for managing [[Azure Resource Manager|ARM]] resources; most user-friendly
		- uses Azure SDK for Go under the hood
	- AzureAD: for managing [[Microsoft Entra ID]] resources
	- AzureDevOps: for managing [[Azure DevOps]] resources
	- AzAPI: for managing Azure [[Resource|resources]] by using the ARM APIs directly; most up-to-date
		- uses direct [[REST]] [[API]] calls to the [[Azure Resource Manager]] REST API
	- github: for managing [[GitHub]]
	- Azure Stack: for managing  [[Azure Stack]] resources