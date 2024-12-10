---
created: 2024-03-14T13:23:04Z
updated: 2024-12-10T08:35:00Z
aliases:
  - "!"
tags:
  - "null"
  - null-safety
  - operator
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/null-forgiving
training: https://learn.microsoft.com/en-us/training/modules/csharp-null-safety
---
- `!` to tell the compiler that we know a value will never be null, even though it could be according to the code
- Ignores the [CS8600 warning](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/compiler-messages/nullable-warnings#possible-null-assigned-to-a-nonnullable-reference)