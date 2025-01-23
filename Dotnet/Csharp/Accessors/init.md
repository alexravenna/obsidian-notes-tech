---
created: 2024-07-17T08:52:22Z
updated: 2025-01-23T13:16:10+01:00
tags:
  - access-control
  - immutability
  - accessor
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/init
---
# Description
- Enforces immutability: once an `init` property has been initialized, its value can't be changed
- An `init` property can only be assigned a value during object construction
- Properties can be initialized by an [[object initializer]] if there is no [[constructor]]