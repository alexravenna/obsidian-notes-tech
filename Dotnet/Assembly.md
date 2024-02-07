---
tags:
  - dotnet
resources:
  - https://learn.microsoft.com/en-us/dotnet/standard/assembly/
---
# Description
- The building block of a [[.NET]] application
- Comes as either:
	- .exe
	- .dll
- Contains:
	- Assembly manifest (required)
	- Type metadata: used for exported types
	- [[MSIL]] code that implements the types
	- Resources
# Manifest
- Every assembly has an assembly manifest file
- Contains metadata describing the contents of the assembly and their relationships
- Contents:
	- The assembly's identity: name and version
	- A table listing all files that make up the assembly
	- A list of external dependencies