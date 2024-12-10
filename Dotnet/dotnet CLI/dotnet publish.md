---
created: 2024-03-20T09:57:57Z
updated: 2024-12-10T08:35:00Z
tags:
  - command
  - compiler
  - dotnet
  - output
documentation:
  - https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-publish
---
# Description
- `dotnet publish` compiles the application and outputs the following assets:
	- [[MSIL]] code in an [[Assembly|assembly]] as a `.dll`
	- A `.deps.json` file that includes all project dependencies
	- A `.runtimeconfig.json` file that specifies:
		- The expected shared runtime
		- Runtime configuration options
	- The application's dependencies, copied from the [[NuGet]] cache