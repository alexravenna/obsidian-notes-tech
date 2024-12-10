---
created: 2024-03-14T08:43:35Z
updated: 2024-12-10T08:35:00Z
tags:
  - "null"
  - nullable
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/nullable-references
specification: https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/proposals/csharp-8.0/nullable-reference-types
training: https://learn.microsoft.com/en-us/training/modules/csharp-null-safety
---
# Description
- [[Reference type|Reference types]] have always been nullable
	- If uninitialized, a reference type is implicitly `null`
- Since C# 8.0 you can express that a reference type *might* be `null`or is *always* non-`null`
	- This allows the compiler to check for you if a `NullReferenceException` might be thrown while de-referencing a `null`
# Nullable Context
- Nullable reference types are enabled through a nullable context
- There are 4 kinds:
	- `disable`
	- `enable`
	- `warnings`
	- `annotations`
- The nullable context can be set:
	- in the `.csproj` file
		- set by default to `enable` in all new project templates for .NET 6.0 and up
	- with the [[compiler directive]] `#nullable