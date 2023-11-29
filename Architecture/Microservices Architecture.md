---
tags:
  - architecture
resources:
  - https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/microservices-architecture
---
- Derived from [[Service-oriented Architecture]]
- Each service runs in its own process
- Processes communicate with each other
	- Common protocols:
		- [[HTTP]]/[[HTTPS]]
		- [[WebSockets]]
		- [[AMQP]]
- Each microservice:
	- represents a specific domain
	- is independently developable and deployable
	- owns its own domain data model and logics
- Microservices can use different programming languages and data storage technologies