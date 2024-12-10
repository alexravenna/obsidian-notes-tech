---
created: 2024-07-17T08:46:10Z
updated: 2024-12-10T08:35:00Z
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/record
resources:
  - https://blog.elmah.io/exploring-c-records-and-their-use-cases/
  - https://stackoverflow.com/questions/65390356/what-are-the-disadvantages-of-using-records-instead-of-classes
---
# Description
- `record class` is synonymous with  `record`;  `class` is optional
- Records possess value equality instead of reference equality: if all the fields of two records have the same values, then they are equal