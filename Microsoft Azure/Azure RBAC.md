---
created: 2024-09-03T20:24:50Z
updated: 2024-12-10T08:34:58Z
documentation:
  - https://learn.microsoft.com/en-us/azure/role-based-access-control/
---
# Description
- [[RBAC]] allows assigning specific permissions to users, groups, [[Service Principal|service principals]] or [[Managed Identity|managed identities]] in [[Microsoft Azure/Azure]]
- Different services offer different roles that can be assigned
- Roles are groups of different permissions
	- There are built-in roles, but custom ones can be created too
- Roles can be assigned with:
	- [[Azure PowerShell]]
	- [[Azure CLI]]
	- [[Azure SDK]]s
	- [[REST]] [[API]]s
- Scope: the set of resources that access applies to
	- Levels:
		- Management group
		- [[Subscription]]
		- [[Resource#Resource Groups|Resource group]]
		- [[Resource]]
# Role Assignment Process
1. Determine who needs access
2. Select the appropriate role
3. Identify the needed scope
4. Check your own prerequisites
5. Assign the role