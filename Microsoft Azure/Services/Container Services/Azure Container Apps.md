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
	- But provides no access to it
- Features:
	- service discovery
	- traffic splitting
	- scaling based on traffic
- 
- 
# Container App Environment
- One or more Container Apps run in an environment, which means they:
	- are in the same virtual network
	- write to the same [[Azure Log Analytics]] workspace
- This offers:
	- HTTPS ingress
	- Service discovery