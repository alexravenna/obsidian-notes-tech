---
created: 2025-03-04T10:31:41+01:00
updated: 2025-03-04T10:34:57+01:00
tags:
  - windows-service
---
# Description
- Get the service
```pwsh
  Get-Service <service_name>
```
- Stop the service
```pwsh
  Stop-Service <service_name>
```
- Delete the service
```pwsh
  sc.exe delete <service_name>
```