---
aliases:
  - "!"
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/null-forgiving
training: https://learn.microsoft.com/en-us/training/modules/csharp-null-safety
tags:
  - "null"
  - null-safety
  - operator
---
- `!` to tell the compiler that we know a value will never be null, even though it could be according to the code
- Ignores the [CS8600 warning](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/compiler-messages/nullable-warnings#possible-null-assigned-to-a-nonnullable-reference)