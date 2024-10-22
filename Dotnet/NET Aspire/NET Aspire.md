---
aliases:
  - .NET Aspire
tags:
  - cloud-native
  - dotnet
resources:
  - https://www.youtube.com/playlist?list=PLdo4fOcmZ0oUfIayQMrRqaSL55Rkck-GD
training:
  - https://learn.microsoft.com/en-us/training/paths/dotnet-aspire/
---
# Description
- A suite of tools for developing distributed, [[cloud-native]] applications with [[NET|.NET]]
- Offers auto-provisioning to [[Azure]]
- Service defaults
- AppHost
	- generates deployment manifest
- Dashboard
# Service Discovery
- Service discovery is automatically configured from AppHost to service projects
# Integrations
- Each integration:
	- is a [[NuGet]] package
	- implements a standard interface to a backing service
- Each integration usually has a hosting package:
	- for use in the AppHost
	- can provision and manage resources
	- can automate infrastructure setup
- And a client package for consuming the resource/dependency
- types:
	- [[Node.js]]
	- [[Python]]
	- [[Docker]]
	- [[NET|.NET]] projects
	- Databases:
		- [[relational]]:
			- [[PostgreSQL]]
			- SQL Database:
				- [[SQL Server]]
				- [[Azure SQL Database]]
			- MySQL
		- [[NoSQL]]:
			- [[MongoDB]]
			- [[Azure Cosmos DB]]
	- Data storage:
		- [[Azure Blob Storage]]
		- [[Azure Queue Storage]]
		- [[Azure Table Storage]]
	- Caching
		-  Redis
			- StackExchange Redis
			- StackExchange Redis output caching
			- StackExchange Redis distributed caching
	- Messaging
		- [[RabbitMQ]]
		- [[Azure Service Bus]]
	- Monitoring and logging
# Tooling
- Project templates
- The .NET Aspire dashboard
	- shows:
		- all [[microservices]]
		- all backing services
		- performance and monitoring tools