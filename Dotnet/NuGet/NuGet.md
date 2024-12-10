---
created: 2023-11-17T14:40:20Z
updated: 2024-12-10T08:34:59Z
tags:
  - dependency-manager
  - dev-tool
  - package-manager
resources:
  - https://learn.microsoft.com/en-us/nuget/
---
# Description
- The primary [[package manager]] for [[NET|.NET]]
# NuGet Package
- `.nupkg` extension
- Single [[ZIP]] file that contains:
	- compiled code ([[DLL]]s)
	- other related files
	- a manifest
# Version Ranges
https://learn.microsoft.com/en-us/nuget/concepts/package-versioning

# Package location
## global-packages
- Packages downloaded by NuGet are installed to `global-packages`
	- When using `PackageReference`: packages are used directly from here
	- When using  `packages.config`: packages are copied from here to the project's `packages` folder
- Windows location: `%userprofile%\.nugetpackages`
- Linux location: `~/.nuget/packages`
## http-cache
- [[Visual Studio]] Package Manager and [[dotnet CLI]] store copies of downloaded packages in a cache for 30 minutes
- Windows location: `%localappdata%\NuGet\v3-cache`
- Linux location: `~/.local/share/NuGet/v3-cache`

# Central Package Management
[.NET Upgrade Assistant Now Supports Upgrading to Centralized Package Mangement - .NET Blog](https://devblogs.microsoft.com/dotnet/dotnet-upgrade-assistant-cpm-upgrade/)