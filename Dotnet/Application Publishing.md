---
created: 2024-05-21T08:31:41Z
updated: 2024-12-10T08:35:00Z
documentation:
  - https://learn.microsoft.com/en-us/dotnet/core/deploying/
---
- Possibilities:
	- with [[Visual Studio]]
	- with the [[dotnet CLI]]: [[dotnet publish]]
- The application can be:
	- *self-contained*: the [[NET runtime|.NET runtime]] libraries are included in the published output
		- produces a platform-/architecture-specific [[Portable Executable|executable]]
		- done by adding the parameters `--self-contained -r <RID>` to `dotnet publish`
	- *framework-dependent:* the .NET runtime has to be installed separately on the target machine
		- done with `dotnet publish`
		- output is cross-platform by default and produces:
			- a cross-platform, framework-dependent binary as a .dll
				- this can be run with the `dotnet` command
			- a platform-specific executable for the current platform
		- output can be platform-specific by specifying an [[Runtime Identifier|RID]] for `dotnet publish` with `-r <RID>`