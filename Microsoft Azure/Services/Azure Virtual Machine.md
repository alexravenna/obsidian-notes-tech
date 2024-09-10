---
aliases:
  - Azure VM
tags:
  - IaaS
---
# Descriptions
- Enables running [[Virtual Machine|virtual machines]] in [[Microsoft Azure/Azure]]
- Virtual machine scale sets: automatically scaled, [[Load balancing|load-balanced]] group of identical VMs
- Virtual machine availability sets: for [[resiliency]] and [[High Availability|high availability]]
	- VMs are grouped into:
		- Update domain: VMs that can be rebooted at the same time
		- Fault domain: by default, there are three fault domains in an availability set, which each have different power and networking resources
- Resources configurable upon provisioning:
	- Size
	- Storage disks
	- Networking