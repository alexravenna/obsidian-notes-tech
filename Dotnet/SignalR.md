---
created: 2023-11-16T08:04:03Z
updated: 2024-12-10T08:34:59Z
aliases:
  - ASP.NET Core SignalR
tags:
  - aspnet-core
  - open-source
  - real-time
  - web
documentation:
  - https://learn.microsoft.com/en-us/aspnet/core/signalr/
training: https://learn.microsoft.com/en-us/training/modules/aspnet-core-signalr/
---
# Description
- An [[API]] that enables real-time communication between web servers and clients for two-way ([[duplex]])  [[RPC]]s
- A **hub**:
	- handles message dispatching between the server and client
	- is exposed through a route, e.g. `https://www.contoso-pizza.com/hubs/orders`
- Messages can be sent to groups, where all users in the group are then notified
- A **group**:
	- has a unique identifier (name)
	- consists of one or more connections
	- is managed by the server
	- is a scoping mechanism
- A **user** can connect from multiple client applications (web browser, mobile app, desktop app, etc.)
- Each client has a unique connection to the server with a unique identifier
- **Events**:
	- are fired by the server
	- are handled by interested clients
	- are subscribed to by clients on their hub's connection
	- can be indirectly triggered by clients calling hub methods, but not directly
## Transports
- SignalR chooses the best transport method
- Listed in graceful fallback order, they are:
	1. [[WebSockets]]
	2. [[Server-sent events]]
	3. Long polling
## Protocols
- The two built-in protocols are:
	- text as JSON (default)
	- binary based on [[MessagePack]]
