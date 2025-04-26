---
created: 2024-04-23T08:22:57Z
updated: 2025-04-10T13:44:52+02:00
---
# Description
- All data is encrypted
- Accessible through [[HTTP]] and [[HTTPS]] through:
	- client libraries
	- a [[REST]] [[API]]
- Scripting supported through:
	- [[Azure PowerShell]]
	- [[Azure CLI]]
- Storage tiers with varying costs, availability and granularity at what level the tier can be set (account or blob level):
	- Hot - for frequently accessed data
	- Cool - for infrequently-accessed data stored for at least 30 days
	- Cold - for infrequently-accessed data stored for at least 90 days
	- Archive - for rarely-accessed data stored for at least 180 days, with flexible latency requirements
- Azure Storage can be mounted as [[Volumes|volumes]] for [[Virtualization/Containers/Docker/Docker|Docker]] [[Container|containers]] through a plugin
# Azure Storage Account
- An Azure Storage account is the top-level container for all Storage [[#Services|services]]
- It has to have a namespace that is unique in Azure
- The account name is included in every object address [[URI]]
# Services
- [[Azure Blob Storage]]
- [[Azure Data Lake Storage]]
- [[Azure Disk Storage]]
- [[Azure Files]]
- [[Azure Queue Storage]]
- [[Azure Table Storage]]
# Access Tiers
- Hot
	- for frequent access
	- default for new [[#Azure Storage Account|Storage accounts]]
- Cool
	- for infrequent access
	- stored for at least 30 days
- Cool
	- for infrequent access
	- stored for at least 90 days
- Archive
	- only for individual block blobs
	- retrieval can take several hours
	- stored for at least 180 days
# Redundancy
- Data is always stored redundantly
## In the primary region
- Data is always replicated synchronously three times in the primary region
- Options for replication in the primary region:
	- Locally redundant storage (LRS) - data replicated three times in a single data center
	- Zone-redundant storage (ZRS) - data replicated across three [[Azure#Physical Infrastructure|Availability Zones]]
## In a secondary region
- Data can be replicated asynchronously to a secondary region
	- Target for data replication is 15 minutes - known as recovery point objective (RPO)
		- There's no [[Service Level Agreement|SLA]] for this
- The secondary region is based on Azure Region Pairs
	- Options:
		- Geo-redundant storage (GRS) - LRS + LRS in a secondary region
		- Geo-zone-redundant storage (GRZS) - ZRS in the primary region + LRS in a secondary region
- Read and write access isn't available in the secondary region unless there is a [[failover]]
	- Or if you enable read access, which makes:
		- read-access geo-redundant storage (RA-GRS)
		- read-access geo-zone-redundant storage (RA-GZRS)
