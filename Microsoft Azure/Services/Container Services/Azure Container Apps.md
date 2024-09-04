---
aliases:
  - ACA
tags:
  - active-di
  - container
  - PaaS
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
- Authentication and authorization:
	- Built-in middleware
		- Runs as a sidecar container on each application replica
	- Uses [[Federated Identity|federated identity]] and supports any number of the following:
		- Microsoft Identity Platform
		- Facebook
		- GitHub
		- Google
		- Twitter
		- Any [[OpenID Connect]] provider
- Offers [[Envoy]] as application gateway
- Compute plan types:
	- Consumption/serverless
		- Limited resources: 4 vCPUs, 8 GiB RAM
		- Free amount of resources/requests
	- Dedicated
		- Workload profiles are defined:
			- Varying amounts of [[CPU]] and [[RAM]]
			- Scale independently
		- Costs:
			- Baseline plan management costs
			- Per CPU/RAM usage

# Container App Environment
- One or more Container Apps run in an environment, which means they:
	- are in the same virtual network
	- write to the same [[Azure Log Analytics]] workspace
- This offers:
	- HTTPS [[ingress]]
	- [[Service discovery]]
# Revisions
- An immutable snapshot of a Container App version
- Certain changes to the App are considered revision-scope changes and trigger generation of a new revision
- Characteristics:
	- Only one revision can be active at the same time
	- External traffic can be routed to different active revisions
	- Revisions can be reverted to
	- Each revision has its own unique name, which is also in the [[URL]]
- Revision modes:
	- single
	- multiple - for [[blue-green deployment]]s
# Secrets
- Container Apps doesn't support [[Azure Key Vault]] integration
	- You have to use the Key Vault SDK in your code
- Changing secrets doesn't trigger a revision change
- Secrets are scoped to an application and not to a revision
- Defined with `--secrets` in the [[Azure CLI]]
# Dapr Integration
- Container Apps provides a managed [[Dapr]] integration
- Dapr can be configured through:
	- CLI
	- [[Infrastructure as Code|IaC]]: [[Bicep]], [[ARM Templates]]
	- The [[Azure portal]]
- Dapr components can be shared across container apps or scoped to specific apps
# KEDA Integration
- [[KEDA]]
# Jobs
