---
created: 2024-03-08T16:15:28Z
updated: 2024-12-10T08:35:00Z
aliases:
  - .NET Aspire
tags:
  - cloud-native
  - dotnet
resources:
  - https://github.com/dotnet-presentations/letslearn-dotnet-aspire
  - https://github.com/dotnet/eshop
  - https://learn.microsoft.com/en-us/samples/browse/?expanded=dotnet&products=dotnet-aspire
  - https://www.youtube.com/playlist?list=PLdo4fOcmZ0oUfIayQMrRqaSL55Rkck-GD
  - https://www.youtube.com/watch?v=4ixWtXK7KzY
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
	- [[Virtualization/Containers/Docker/Docker|Docker]]
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