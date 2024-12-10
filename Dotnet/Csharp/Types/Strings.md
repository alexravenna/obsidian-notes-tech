---
created: 2024-04-22T07:15:55Z
updated: 2024-12-10T08:35:00Z
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
# Verbatim String Interpolation
- Verbatim string interpolation combines [[#Verbatim String Literals]] and [[#String Interpolation]] to allow you to create dynamic, multi-line, non-escaped text
- Can be written as either `$@"..."` or `@$"..."`
  ```csharp
var myInfo = (firstName: "Alex", lastName: "Ravenna", age: 36);
string myInfoString = $@"My name is {myInfo.firstName} {myInfo.lastName}.
I am {myInfo.age} years old."
```