---
created: 2024-08-27T07:44:40Z
updated: 2024-12-10T08:35:00Z
documentation:
  - https://learn.microsoft.com/en-us/ef/core/cli/
---

# Package Manager Console tools
- #caveat Make sure that you're using [[PowerShell|PowerShell Core 7]]
	- PowerShell 5 can't access v3 of the [[NuGet]] feed
	- Check this with `$PSVersionTable`
```powershell
Install-Package Microsoft.EntityFrameworkCore.Tools
Update-Package Microsoft.EntityFrameworkCore.Tools
```
# .NET CLI
```
dotnet tool install --global dotnet-ef
dotnet tool update --global dotnet-ef
```