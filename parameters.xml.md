---
created: 2023-11-15T09:36:34Z
updated: 2024-12-10T08:27:06Z
tags:
  - file
  - XML
resources:
  - https://learn.microsoft.com/en-us/azure/devops/pipelines/tasks/transforms-variable-substitution
---
- Used by msdeploy.exe
- Enables [[XML]] transformation and [[XML]]  variable substitution
	- variable substitution: use a placeholder, e.g. `__UserName__` and have it be replaced with `alexravenna` at deployment
- For use with e.g. [[Web.config]] files
- Can be used in [[Azure App Service Deploy]] and [[IIS WebApp Deploy]]