---
created: 2023-12-04T15:05:36Z
updated: 2024-12-10T08:35:00Z
aliases:
  - ??
tags:
  - "null"
  - null-safety
  - operator
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/null-coalescing-operator
specification: https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/expressions#1215-the-null-coalescing-operator
related to: "[[Null-coalescing assignment operator]]"
---
- `??` to check if a value is null and if it is not, then use its value
- Returns the value of the left-hand operand if it isn't `null`; otherwise, the right-hand operand is evaluated
- If the left-hand operand is *non*-null, the right-hand operand isn't evaluated
- #Basically: it provides an alternate value in case the expression evaluates to `null`