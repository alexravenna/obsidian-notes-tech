---
created: 2024-03-14T13:33:03Z
updated: 2025-08-12T22:43:20+02:00
aliases:
  - ?.
tags:
  - "null"
  - null-safety
  - operator
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/member-access-operators#null-conditional-operators--and-
training: https://learn.microsoft.com/en-us/training/modules/csharp-null-safety
---
- `?.` to check if a value/property is `null` before we try to dereference it
	- If it is, use the `default` value of the object
	- If it isn't, allow dereferencing
- Example:
  ```csharp
  FooBar fooBar = null; // Conditionally dereference variable.
  var str = fooBar?.ToString();
  Console.Write(str);
  ```
	- Without the `?`, a `NullReferenceException` would have been thrown because we tried to access a property on a `null` object