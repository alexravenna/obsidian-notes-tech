---
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