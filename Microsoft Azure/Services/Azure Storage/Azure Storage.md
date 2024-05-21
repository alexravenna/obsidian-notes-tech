# Description
- An Azure Storage account has to have a namespace that is unique in Azure
- Storage tiers:
	- Hot
	- Cool
	- Archive
- Azure Storage can be mounted as [[Volumes|volumes]] for [[Docker]] [[Container|containers]] through a plugin
# Services
- [[Azure Blob Storage]]
- [[Azure Data Lake Storage]]
- [[Azure Disk Storage]]
- [[Azure Files]]
- [[Azure Queue Storage]]
- [[Azure Table Storage]]
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
