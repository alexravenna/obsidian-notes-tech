---
created: 2024-09-16T10:37:43Z
updated: 2024-12-10T08:34:58Z
resources:
  - https://learn.microsoft.com/en-us/graph/api/resources/application
---
# Application object
- A template for creating [[service principal]] objects
- A global representation of an application across all [[Tenant|tenants]]
- Has common and default properties for all [[Service Principal|service principal]] objects
- What an application is scoped to
- Resides in the [[Microsoft Entra]] tenant where the [[Application registration|app registration]] took place: the home tenant
- Describes:
	- how a service can issue tokens to access the application
	- resources the application may need to access
	- the actions the application can take