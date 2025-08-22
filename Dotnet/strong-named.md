---
created: 2025-08-19T19:00:03+02:00
updated: 2024-12-10T12:57:41Z
tags:
  - assembly
documentation:
  - https://learn.microsoft.com/en-us/dotnet/standard/assembly/strong-named
---
# Description
- A strong-named [[Assembly|assembly]] has a unique identity to help prevent assembly conflicts
- The identity is created using a [[public key|public]]/[[private key]] pair: [How to: Create a public-private key pair - .NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/assembly/create-public-private-key-pair)
- How to strong-name:
	- With the Strong Name tool (Sn.exe): [Sn.exe (Strong Name Tool) - .NET Framework | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/framework/tools/sn-exe-strong-name-tool)
	- With various Visual Studio tools: [How to: Sign an assembly with a strong name - .NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/assembly/sign-strong-name)
- All assemblies in [[NET Core|.NET Core]] are strong-named
- Having to strong-name an assembly is more the exception than the rule