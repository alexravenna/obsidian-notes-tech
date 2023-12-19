---
tags:
  - csharp
  - method
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/extension-methods
---
- A way to add additional methods to a [[class]] or [[interface]]
- Defined as [[static]] methods but called as if they belong to the class [[instance]]
- Often used in [[LINQ]]
- Example definition:
```csharp
public static class StringExtensions
{
	public static void LogString(this string str)
	{
		Console.WriteLine(str);
	}
}
```
- Example usage:
```csharp
var MyString = "Hello World";
MyString.LogString();
```
- The extension method can still be called as a static method:
```csharp
var MyString = "Life is great";
StringExtensions.LogString(MyString);
```