---
created: 2025-05-10T12:29:23+02:00
updated: 2025-07-04T07:58:45+02:00
---
# Description
- Acts as a [[VPN]] from an [[Azure Virtual Network]]
- Enables the connection types:
	- site-to-site: [[on-premise]] network to [[virtual network]]s
	- point-to-site: individual devices to [[virtual network]]s
	- network-to-network: [[virtual network]]s to other [[virtual network]]s
- Only one can be deployed in each [[Azure Virtual Network]]
- Has two types of [[VPN]]:
	- policy-based: determines which traffic to [[encrypt]] based on [[IP address]]
	- route-based: uses [[IP routing]] to determine which [[IPSec tunnel]] to use
		- is more resilient to [[topology]] changes