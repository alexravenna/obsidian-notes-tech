---
created: 2025-08-12T22:43:09+02:00
updated: 2025-08-12T22:51:51+02:00
tags:
  - csharp
  - operator
aliases:
  - ^
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/member-access-operators#index-from-end-operator-
---
# Description
- Used to signify the element count from the last element in a sequence
- The sequence must have an `int` property `Count` or `Length`
- `MyArray[^1]` is equivalent to `MyArray[MyArray.Length - 1]`
- `MyArray[^2]` is equivalent to `MyArray[MyArray.Length - 2]` and so on