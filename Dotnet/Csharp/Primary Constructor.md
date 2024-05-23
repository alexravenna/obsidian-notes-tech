---
tags:
  - constructor
documentation:
  - https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/instance-constructors#primary-constructors
---
- Available starting in [[Csharp|C#]] 12
- For [[class|classes]] and [[structs]]
- Parameters are defined in the class definition instead of in a separate `constructor` definition
- Parameters are necessary for any instance of the type
- Example:
  ```csharp
	public class NamedItem(string name)
	{
	    public string Name => name;
	}