---
tags:
  - active-di
  - container
  - serverless
documentation:
  - https://learn.microsoft.com/en-us/azure/container-apps/
training:
  - https://learn.microsoft.com/en-us/training/paths/deploy-cloud-native-applications-to-azure-container-apps/
---
# Description
- A serverless platform
- Based on [[Container|containers]]
- Powered by [[Kubernetes]]
	- But provides no access to it directly
- Features:
	- service discovery
	- traffic splitting
	- scaling based on traffic
- [[Container Image|Images]] must be based on the `linux/amd64` platform
- Multiple containers can run in one container app
	- They share hard disk and network resources
	- They have the same application lifecycle
	- This can be used to implement the [[Sidecar|sidecar pattern]]
- Images can be pulled from [[Container Registry|container registries]]
# Container App Environment
- One or more Container Apps run in an environment, which means they:
	- are in the same virtual network
	- write to the same [[Azure Log Analytics]] workspace
- This offers:
	- HTTPS ingress
	- Service discovery