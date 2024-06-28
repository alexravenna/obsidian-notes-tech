---
tags:
  - constant
  - readonly
  - static
resources:
  - https://stackoverflow.com/questions/3190870/const-string-vs-static-readonly-string-in-c-sharp
  - https://www.stum.de/2009/01/14/const-strings-a-very-convenient-way-to-shoot-yourself-in-the-foot/
---
- `const` 
	- a constant that is set at compile-time
	- can only be initialized inline and with other constants or literals
- `static readonly`:
	- a [[field]] that gets evaluated at runtime
	- can be initialized in a [[static]] [[constructor]]
- Both fields can't have their values changed once initialized