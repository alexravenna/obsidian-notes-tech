---
tags:
  - placeholder
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/functional/discards
---
- `_`
- Used as a placeholder value for a return value you don't want to use
- Often used when [[deconstructing]] [[tuples]]:
```csharp
  (_, _, area) = city.GetCityInformation(cityName);
```
- Also used when an `out` parameter doesn't need to be used:
```csharp
  if (DateTime.TryParse(dateString, out _)) Console.WriteLine($"'{dateString}': valid");
```