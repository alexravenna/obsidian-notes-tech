---
resources:
  - https://azure.microsoft.com/en-us/solutions/cloud-native-apps/
  - https://learn.microsoft.com/en-us/dotnet/architecture/cloud-native/
  - https://learn.microsoft.com/en-us/shows/the-cloud-native-show/
training:
  - https://learn.microsoft.com/en-us/training/paths/deploy-cloud-native-applications-to-azure-container-apps/
---
# Description
- An approach to developing and running applications in cloud environments
- They should be:
	- scalable
	- distributed/distributable
	- composed of loosely-coupled services
- Services may not necessarily come from you (i.e. managed services)
- Often associated with or implies a [[Microservices Architecture|microservices architecture]]
- Six common characteristics:
	- use cloud infrastructure
	- implemented as microservices
	- components are run in [[Container|containers]]
	- backing services ([[Database|databases]], [[Caching|caching services]], etc.) can be used
	- conformity to the [[Twelve-Factor App]] methodology
	- deployment and [[provisioning]] done through [[Infrastructure as Code]]