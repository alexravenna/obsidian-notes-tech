---
tags:
  - dev-tool
  - dependency-manager
resources:
  - https://learn.microsoft.com/en-us/nuget/
---
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