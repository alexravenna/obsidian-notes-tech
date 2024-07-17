---
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/record
resources:
  - https://stackoverflow.com/questions/65390356/what-are-the-disadvantages-of-using-records-instead-of-classes
---
- `record class` is synonymous with  `record`;  `class` is optional
- Records possess value equality instead of reference equality: if all the fields of two records have the same values, then they are equal