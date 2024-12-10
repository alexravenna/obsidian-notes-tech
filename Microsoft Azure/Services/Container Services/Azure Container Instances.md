---
created: 2024-07-19T13:59:34Z
updated: 2024-12-10T08:34:57Z
aliases:
  - ACI
tags:
  - PaaS
training:
  - https://learn.microsoft.com/en-us/training/modules/create-run-container-images-azure-container-instances/
---
# Description
- "`docker run`" in the cloud
- [[Linux]] and [[Windows]] [[Container|containers]]
- Container groups can be exposed publicly with an [[IP Address|IP address]] and an [[FQDN]]
- [[Azure Files]] shares can be mounted directly to a container
- Container group:
	- The top-level [[Resource|resource]] for ACI
	- Containers in a container group share:
		- a lifecycle
		- resources
		- local network
		- storage volumes
	- The containers are all scheduled on the same host machine
	- Multi-container groups only support Linux containers
# Deployment
- Container groups can be deployed with:
	- an [[ARM Templates|ARM template]] - better for when additional resources are necessary
	- a [[YAML]] file - better when only container instances are used
# Networking
- Container groups share:
	- an IP address
	- a [[port namespace]]; [[port mapping]] isn't supported
- Containers in a group can communicate with each other on [[localhost]] on their [[exposed]] [[ports]]
# Storage
- Supported volumes:
	- Azure File share
	- Secret
	- Empty directory
	- Cloned [[Git]] [[Repository|repo]]
# Restart Policy
- Specified as `restart-policy` when using [[Azure CLI]]
- Policies:
	- Always: default
	- Never
	- OnFailure
# Using File Share
- Azure Files shares are accessible with [[SMB]]
- Files shares can only be mounted to Linux [[!db/resources/github/containers/containers|containers]]
- The Linux container must run as [[root]]