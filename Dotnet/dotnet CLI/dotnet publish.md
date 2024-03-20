---
documentation:
  - https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-publish
tags:
  - dotnet
  - command
  - compiler
  - output
---
# Description
- `dotnet publish` compiles the application and outputs the following assets:
	- [[MSIL]] code in an [[Assembly|assembly]] as a `.dll`
	- A `.deps.json` file that includes all project dependencies
	- A `.runtimeconfig.json` file that specifies:
		- The expected shared runtime
		- Runtime configuration options
	- The application's dependencies, copied from the [[NuGet]] cache