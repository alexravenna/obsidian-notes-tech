---
tags:
  - azure
  - policy
documentation:
  - https://learn.microsoft.com/en-us/azure/governance/policy/
training:
  - https://learn.microsoft.com/en-us/training/modules/intro-to-azure-policy/
---
# Description
- Enables compliance enforcement: create, assign and manage policy definitions
- For already existing [[Resource|resources]] and resources during deployment
- For all resource types
- Allows control over:
	- The types of [[Resource|resources]] that can be provisioned
	- The locations where resources can be provisioned
- Built-in policies:
	- Allowed locations
	- Allowed virtual machine size [[SKU]]s
- Custom policies also possible
- Allows noncompliance remediation
- Written in [[JSON]]
- Initiative: a set or group of policies
	- Also written in JSON
- Definitions: built-in or custom initiatives and policies that are available
- Policy exemptions can be configured based off of hierarchy or for individual resources
- Free for [[Microsoft Azure/Azure]] resources but not for [[Azure Arc]] resources
- [[Repository]] for built-in policies: [Azure/azure-policy: Repository for Azure Resource Policy built-in definitions and samples (github.com)](https://github.com/Azure/azure-policy)