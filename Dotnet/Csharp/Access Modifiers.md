---
created: 2024-06-26T07:47:49Z
updated: 2024-12-10T08:35:00Z
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/access-modifiers
resources:
  - https://stackoverflow.com/questions/3763612/default-visibility-for-c-sharp-classes-and-members-fields-methods-etc
---
# Defaults
# Top-Level Types
- The default access modifier is `internal`
- Only `internal` or `public` are possible
## Nested Types
| **Members of** | **Default member accessibility** | **Allowed declared accessibility of the member**                                                             |
| -------------- | -------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| `enum`         | `public`                         | None                                                                                                         |
| `class`        | `private`                        | `public`  <br>`protected`  <br>`internal`  <br>`private`  <br>`protected internal`  <br>`private protected`  |
| `interface`    | `public`                         | `public`  <br>`protected`  <br>`internal`  <br>`private`*  <br>`protected internal`  <br>`private protected` |
| `struct`       | `private`                        | `public`  <br>`internal`  <br>`private`                                                                      |
