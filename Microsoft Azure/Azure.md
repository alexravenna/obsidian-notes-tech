---
created: 2023-11-13T10:59:49Z
updated: 2024-12-10T08:34:58Z
tags:
  - cloud
  - microsoft
  - platform
training: https://learn.microsoft.com/en-us/training/modules/describe-core-architectural-components-of-azure/
BC-tag-note-tag: "#azure"
BC-tag-note-field: down
---
# Description
- The cloud platform from [[Microsoft/Microsoft|Microsoft]]
- Offers more than 100 services spanning:
	- Running apps/[[VM]]s
	- Storage, i.e. [[Database|databases]]
	- [[IoT]]
	- [[Machine Learning|ML]]
- Global
# Physical Infrastructure
- Azure Regions
	- Contain at least one datacenter
	- Availability Zones exist in some regions
		- Consist of one or more independent datacenters
		- Offer resiliency and redundancy if one zone goes down
	- Region pairs exist for most regions
		- The regions are at least 300 miles away from each other
		- Regions act as fallbacks and backups for each other
# Management Infrastructure
- Management group
	- (Potential other management groups - up to 6 levels)
		- [[Subscription]]
			- [[ Resource|Resource Group]]
				- [[Resource]]
# Services
- [[Azure Active Directory B2C]]
- [[Azure Container Registry]]
- [[Azure App Service]]
- [[Azure Cosmos DB]]
- [[Azure SQL Database]]
- [[Azure Storage#Services|Azure Storage Services]] 
- [[Azure Key Vault]]
- [[Azure Resource Manager]]
- [[Azure Monitor]]
- [[Azure Kubernetes Service (AKS)]]
- [[Azure Functions]]
- [[Azure Sentinel]]