---
created: 2025-01-23T13:10:08+01:00
updated: 2025-01-23T13:11:58+01:00
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/object-and-collection-initializers
---
# Description
- Allow [[instantiation]] and member assignment in one [[statement]]
```csharp
Cat cat = new Cat { Age = 10, Name = "Fluffy" };
Cat sameCat = new Cat("Fluffy"){ Age = 10 };
```