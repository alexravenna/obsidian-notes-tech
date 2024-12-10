---
created: 2023-11-13T10:59:49Z
updated: 2024-12-10T08:34:58Z
aliases:
  - ACR
tags:
  - azure
  - registry
homepage:
  - https://azure.microsoft.com/en-us/products/container-registry/
documentation:
  - https://learn.microsoft.com/en-us/azure/container-registry/
training:
  - https://learn.microsoft.com/en-us/training/modules/configure-azure-container-registry-container-app-deployments/
  - https://learn.microsoft.com/en-us/training/modules/publish-container-image-to-azure-container-registry/
---
# Description
- A managed, private [[Container Registry|container registry]] based on [[Docker Registry]] 2.0
- Three tiers:
	- Basic
	- Standard
	- Premium
- Can contain [[Linux]] and [[Windows]] [[Container Image|images]]
- Can also store:
	- [[Virtualization/Kubernetes/Helm]] [[charts]]
	- images built according to the [[image-spec|OCI Image Specification]]
- Uses  [[MS Defender for Containers]]
	- [[Defender for Cloud]] is optional
- Features:
	- encryption-at-rest (all tiers)
	- data is stored in registry's region
	- geo-replication (optional)
	- zone redundancy (Premium only)
- Fully qualified name: `<registry-name>.azurecr.io`
# Tasks
- Enable offloading image building and pushing to the registry
	- Quick tasks accomplish this
- Can automatically trigger image builds upon [[VCS]] changes
- Possible triggers:
	- source code update
	- base image update
	- schedule
- Multi-step tasks allow more complex workflows
	- Containers are used as execution environments
# Commands
- With the [[Azure CLI]]:
	- Creation:
	  `az acr create --resource-group RG1 --name mycontainerregistryapl2003 --sku Premium`