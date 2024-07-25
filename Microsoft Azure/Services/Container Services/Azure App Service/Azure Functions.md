---
tags:
  - azure
  - compute
  - event-driven
  - PaaS
  - serverless
  - service
documentation:
  - https://learn.microsoft.com/en-us/azure/azure-functions/
training:
  - https://learn.microsoft.com/en-us/training/modules/intro-azure-functions/
  - https://learn.microsoft.com/en-us/training/paths/implement-azure-functions/
---
# Description
- A serverless solution for running compute workloads: Functions-as-a-Service
- For event-driven applications
- Functions can be written in many different languages:
	- [[Csharp|C#]]
	- [[Java]]
	- [[JavaScript]]/[[TypeScript]]
	- [[PowerShell]]
	- [[Python]]
	- For other languages with a custom handler
- Function app:
	- The runtime/execution context for a function
	- A way to organize and manage functions
	- All functions in a function app:
		- share the same settings and connections
		- must be written in the same language
- Has built-in integration with [[Azure Monitor Application Insights|Application Insights]]
- Built on the [[WebJobs SDK]]
- Can integrate with [[Azure Logic Apps|Logic Apps]]
- Deployment slots:
	- Enable different environments for running different instances of a function app
- Require an [[Azure Storage]] account for managing triggers and logging executions
	- The storage account must support [[Azure Blob Storage|Azure Blob]], [[Azure Queue Storage|Queue]], [[Azure Files||Files]], and [[Azure Table Storage|Table]] storage
	- Code files are stored on [[Azure Files]] shares
- Three levels of protection are available for functions triggered by HTTP requests:
	- Anonymous - any user can trigger the function
	- Function - the request has to provide a certain key
	- Admin - same as Function level but uses an admin key
- Other types of triggers require connection strings as form of protection
# Triggers
- Triggers start the execution of functions
- Functions must have exactly one
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
	- declarative
- Both input and output bindings can be used at the same time
- Input bindings pass data into the function
- Output bindings write data from the function to a data destination
# Hosting Plans
- Consumption plan
	- You pay (for compute) only when functions are running
	- For intermittent usage
	- Has limit on execution time
- Premium plan
	- Functions are kept initialized -> no idling
- Dedicated plan
	- For when functions need to run continuously
- In all plans, functions scale automatically, with varying levels of control over how
	- Scaling occurs by adding more function app instances
- Functions can also be hosted in:
	- [[App Service Environment|ASE]]
	- [[Kubernetes]] through [[KEDA]]
# Development
- Azure Functions Core Tools:
	- Used to run functions locally
- function.json
	- Defines configuration settings for a function, such as:
		- the trigger
		- bindings
	- Generated automatically from annotations/attributes in compiled languages
	- Must be created for scripting languages
- host.json
	- In the root project folder
	- Contains runtime-specific configurations
# Isolated worker model vs. in-process model
- Support for the in-process model will end on November 10, 2026: [Retirement: Support for the in-process model for .NET apps in Azure Functions ends 10 November 2026. | Azure updates | Microsoft Azure](https://azure.microsoft.com/en-us/updates/retirement-support-for-the-inprocess-model-for-net-apps-in-azure-functions-ends-10-november-2026/)
- Link: [Differences between in-process and isolate worker process .NET Azure Functions | Microsoft Learn](https://learn.microsoft.com/en-us/azure/azure-functions/dotnet-isolated-in-process-differences)