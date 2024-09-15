---
homepage:
  - https://azure.microsoft.com/en-us/products/api-management/
documentation:
  - https://learn.microsoft.com/en-us/azure/api-management/
resources:
  - https://learn.microsoft.com/en-us/azure/well-architected/service-guides/api-management/reliability
training:
  - https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-api-management/
---
# Description
- An [[API]] lifecycle management service
- A façade for your APIs
- Developed/maintained by [[Azure API Platform]]
- Three main components:
	- Gateway
	- Single administration interface
	- Developer portal
- Several service tiers available
- Products:
	- A group of APIs that share their configuration
	- All APIs in a product can be accessed with a single subscription key
- Revisions and versions:
	- Revision: a minor, nonbreaking change
	- Version: a major, breaking change
	- Multiple versioning schemes are offered
	- Multiple versions can be enabled at once
- Supported Azure monitoring services:
	- [[Azure Monitor Logs]]
	- [[Azure Monitor Application Insights|Application Insights]]
	- [[Azure Event Hub]]s
# Gateway
- It:
	- verifies subscription keys and other credentials
	- enforces usage policies
	- routes calls to appropriate [[backend]] servers
	- caches backend responses
	- collects call metadata
# Administration Interface
- Allows you to:
	- define/import API specifications:
		- [[OpenAPI]]
		- [[SOAP]]
		- [[WebSocket]]
		- [[GraphQL]]
		- or import instances of [[Azure]] services
	- set usage policies: quotas, rate limits
	- set security policies
	- package APIs into products
	- manage users
	- manage API revisions and versions
	- run analytics on API metadata
# Developer Portal
- Allows developers to:
	- review documentation for your APIs
	- try out APIs
	- review code samples in different [[programming languages]]
	- subscribing to an API and getting a subscription key
	- run analytics on developer's usage
# Policies
- Policy: setting or action that controls the behavior of an API
- Policy categories:
	- Access restriction
	- [[Authentication]]
	- [[Caching]]
	- Validation
- Policy definitions:
	- [[XML]] documents with statements defining policies and their parameters
	- can be set for different stages in the request-response pipeline:
		- inbound
		- outbound