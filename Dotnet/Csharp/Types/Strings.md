---
created: 2024-04-22T07:15:55Z
updated: 2025-02-10T09:40:29+01:00
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/strings/
---

# Description
- Strings are [[Immutable|immutable]]
	- When a string appears to be modified, a copy is actually created and the original will be released up for [[Garbage-collected|garbage collection]]
- `String.Empty` is a constant for the zero-length string `""`
- Certain characters require [[escaping]] in order to be displayed correctly, including:
	- '
	- "
	- \
# Verbatim String Literals
- Verbatim string literals can display multi-line strings and don't require escaping certain characters
```csharp
  string path = @"C:\Users\alexravenna\Documents\";
  string multiline = @"This text
   is mutiline and
   contains a ""quote""";
```
# Raw String Literals
- Since C# 11
- Raw string literals can display multi-line strings and don't require using *any* escape characters
- They start and end with `"""`:
	- Single-line strings: both on the same line
	- Multi-line strings: each on their own line
```csharp
 string multiline = """
	 This text 
	 is mutiline and
	 contains a quote: "Jeder ist sein eigenes Glückes Schmied."
	 """;
```
# String Interpolation
- Allows you to embed dynamic content in a string at run time
```csharp
var myInfo = (firstName: "Alex", lastName: "Ravenna", age: 36);
System.Console.WriteLine($"My name is {myInfo.firstName} {myInfo.lastName} and I am {myInfo.age} years old.");
```
## Format string component
- Optional
- Specifies how the string should be formatted depending on whether the string is:
	- numeric
		- standard: [Standard numeric format strings - .NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/base-types/standard-numeric-format-strings)
		- custom: [Custom numeric format strings - .NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/base-types/custom-numeric-format-strings)
	- a [[DateTime]] object
		- standard: [Standard date and time format strings - .NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings)
		- custom: [Custom date and time format strings - .NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/base-types/custom-date-and-time-format-strings)
	- an [[enumeration]] value: [Enumeration format strings - .NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/base-types/enumeration-format-strings)
- The default is `G` for general
- Enum example
```csharp
Console.WriteLine($"The given shoe is not of the type {ShoeType.Sneaker:G}.")
// > The given shoe is not of the type Sneaker.
```

# Verbatim String Interpolation
- Verbatim string interpolation combines [[#Verbatim String Literals]] and [[#String Interpolation]] to allow you to create dynamic, multi-line, non-escaped text
- Can be written as either `$@"..."` or `@$"..."`
  ```csharp
var myInfo = (firstName: "Alex", lastName: "Ravenna", age: 36);
string myInfoString = $@"My name is {myInfo.firstName} {myInfo.lastName}.
I am {myInfo.age} years old."
```