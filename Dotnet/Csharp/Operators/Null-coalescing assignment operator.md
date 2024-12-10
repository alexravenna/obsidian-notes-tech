---
created: 2024-04-25T07:36:23Z
updated: 2024-12-10T08:35:00Z
aliases:
  - ??=
tags:
  - "null"
  - assignment
  - null-safety
  - operator
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/null-coalescing-operator
related to: "[[Null-coalescing operator]]"
---
-  `??=` assigns the left-hand operand to the right-hand operand only if the left-hand operand evaluates to null
- If the left-hand operand evaluates to *non*-null, the right-hand operand is not evaluated
- #Basically, it can be used to simplify an `if` condition containing a null check:
  ```csharp
  int? myValue = null;
  
  if (myValue == null) myValue = 42;
  // becomes
  myValue ??= 42
```