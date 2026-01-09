---
created: 2024-09-03T20:24:50Z
updated: 2024-12-10T08:34:58Z
documentation:
  - https://learn.microsoft.com/en-us/azure/role-based-access-control/
---
# Description
- [[RBAC]] allows assigning specific permissions to users, groups, [[Service Principal|service principals]] or [[Managed Identity|managed identities]] in [[Azure]]
- Different services offer different roles that can be assigned
- Roles are groups of different permissions
	- There are built-in roles, but custom ones can be created too
		- Reader
		- Contributor
		- Owner
- Roles can be assigned with:
	- [[Azure PowerShell]]
	- [[Azure CLI]]
	- [[Azure SDK]]s
	- [[REST]] [[API]]s
- Scope: the set of resources that access applies to
	- Levels:
		- [[management group]]
		- [[subscription]]
		- [[Resource#Resource Groups|Resource group]]
		- [[Resource]]
- Scope access is hierarchical, e.g.
	- an Owner role in a [[management group]] grants the Owner role to all [[subscription]]s in that group
- Relationship between roles and scopes:
	- A user, admin, observer, automated process or any group of these is assigned a specific role for a specific scope
# Role Assignment Process
1. Determine who needs access
2. Select the appropriate role
3. Identify the needed scope
4. Check your own prerequisites
5. Assign the role