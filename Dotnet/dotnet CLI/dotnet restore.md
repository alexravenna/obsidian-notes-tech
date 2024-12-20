---
created: 2024-03-20T10:09:38Z
updated: 2024-12-10T08:35:00Z
tags:
  - command
  - dotnet
  - nuget
documentation:
  - https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-restore
---
# Description
- `dotnet restore`:
	- looks for [[NuGet]] dependencies of the project and downloads them if necessary
	- ensures that all dependencies are compatible with each other
- `dotnet restore` often doesn't need to be called explicitly, since many other [[dotnet CLI]] commands run it implicitly:
	- [[dotnet publish]]
		- this has the `--no-restore` flag to prevent this implicit restoring