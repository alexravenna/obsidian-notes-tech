---
created: 2024-06-18T07:18:21Z
updated: 2024-12-10T08:34:58Z
tags:
  - azure
  - cache
  - redis
homepage:
  - https://azure.microsoft.com/en-us/products/cache/
documentation:
  - https://learn.microsoft.com/en-us/azure/azure-cache-for-redis/
training:
  - https://learn.microsoft.com/en-us/training/modules/develop-for-azure-cache-for-redis/
  - https://learn.microsoft.com/en-us/training/modules/intro-to-azure-cache-for-redis/
  - https://learn.microsoft.com/en-us/training/modules/optimize-your-web-apps-with-redis/
---
# Description

- Offers [[OSS]] [[Redis]] or [[Redis Enterprise]] as a managed service
- Offers a  Console in the [[Azure portal]] for interacting with the database:
  ![[Pasted image 20240619123342.png]]
- [[Redis Insight]] can also be configured to connect to an Azure Cache for Redis
- Offered in five tiers (the last two use Redis Enterprise):
	- Basic
	- Standard
	- Premium
	- Enterprise
	- Enterprise Flash
# Use Cases
- Distributed [[cache]]
	- Frequently-accessed data is copied to a cache instead of being stored in a traditional database
	- This reduces load on the database and decreases latency for accessing the data
- Session store
	- Store and access temporary user session data like [[cookies]]
- Message broker
	- Azure Cache for Redis can be used as a message broker in a [[publish-subscribe|publish/subscribe]] or [[queue]] architecture for secure (with [[TLS]]) [[asynchronous]] communication
	- Useful for[[Microservices|microservices]]
- Cloud migration
	- [[on-premise|On-premise]] Redis can easily be migrated to Azure Cache for Redis
		- An RDB file exported from Redis can be imported