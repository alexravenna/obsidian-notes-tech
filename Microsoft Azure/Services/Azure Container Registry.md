---
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
  - https://learn.microsoft.com/en-us/training/modules/publish-container-image-to-azure-container-registry/
---
# Description
- A managed, private [[Container Registry|container registry]] based on [[Docker Registry]] 2.0
- Three tiers:
	- Basic
	- Standard
	- Premium
- Can contain [[Linux]] and [[Windows]] images
- Can also store:
	- [[Helm]] [[charts]]
	- images built according to the [[image-spec|OCI Image Specification]]
- Uses  [[MS Defender for Containers]]
# Tasks
- Can automatically trigger [[Container Image|image]] builds upon [[VCS]] changes