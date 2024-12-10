---
created: 2024-02-12T08:04:06Z
updated: 2024-12-10T08:34:57Z
aliases:
  - AKS
tags:
  - azure
  - kubernetes
homepage:
  - https://azure.microsoft.com/en-us/products/kubernetes-service/
training:
  - https://learn.microsoft.com/en-us/training/modules/intro-to-azure-kubernetes-service/
---
# Description
- Fully-managed [[Kubernetes]] service
	- Not a full [[PaaS]] - much administration still necessary, e.g. worker nodes
- Can be created with:
	- [[Azure CLI]]
	- [[Azure portal]]
- Default Initial node pool size is 2; at least is recommended for production
- Supports:
	- [[Virtualization/Kubernetes/Helm]]
	- [[Draft]]
	- [[Kubernetes Extension for Visual Studio Code]]
	- [[Visual Studio Kubernetes Tools]]
- Supports [[Linux]] and [[Windows]] nodes
- Has to cluster autoscaling options:
	- horizontal pod autoscaler (HPA)
	- cluster autoscaler