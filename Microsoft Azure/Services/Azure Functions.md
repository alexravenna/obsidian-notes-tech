---
tags:
  - serverless
  - compute
  - service
  - event-driven
---
# Description
- A serverless solution for running 
- Functions can be written in many different languages:
	- [[Csharp|C#]]
	- [[Java]]
	- [[JavaScript]]
	- [[PowerShell]]
	- For other languages with a custom handler
# Triggers
- Triggers start the execution of Functions
- Trigger types:
	- Storage - listen to events from [[Azure Cosmos DB|Cosmos DB]] and others
	- Events - [[Azure Event Grid|Event Grid]] and [[Azure Event Hub|Event Hub]] events
	- HTTP codes - from web requests and webhooks
	- Queues - process queue messages
	- Timer - run at a specific time or time interval
# Bindings
- Bindings are:
	- used for connecting to data sources (instead of using a client [[SDK]])
	- connection code you don't have to write
- Input bindings pass data into the function
- Output bindings write data from the function to a data destination

# Hosting Plans

# Isolated worker model vs. in-process model