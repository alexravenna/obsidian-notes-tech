---
created: 2024-03-21T11:45:37Z
updated: 2024-12-10T08:34:54Z
aliases:
  - Kubernetes-based Event-Driven Autoscaler
tags:
  - cncf-graduated
  - event-driven
  - kubernetes
  - scaling
homepage:
  - https://keda.sh/
github: https://github.com/kedacore/keda
documentation:
  - https://keda.sh/docs/
---
# Description
- [[vendor-neutral|Vendor-neutral]], [[Cloud-agnostic|cloud-agnostic]]
- 35+ event sources:
	- [[HTTP]] (1)
	- Event-driven, e.g.: (1)
		- [[Azure Service Bus]]
		- [[RabbitMQ]]
		- [[Redis]]
	- [[CPU]] (2)
	- [[Memory]] (2)
- 1. Support for scale to zero and specifying max/minimum replicas
- 2. Support specifying max/minimum replicas