---
homepage:
  - https://learn.microsoft.com/en-us/powershell/
github: https://github.com/PowerShell/PowerShell
documentation:
  - https://learn.microsoft.com/en-us/powershell/scripting/overview
tags:
  - shell
  - command-line
  - cross-platform
---
# Description
- Separate from [[Windows PowerShell]]
- Replaces [[cmd.exe]]
- Consists of:
	- [[command-line shell]]
	- [[scripting]] language
	- configuration management framework: [[DSC]]
- Built on [[NET Core|.NET Core]]
# cmdlets
- A compiled command
- Can be developed in [[.NET]] or [[NET Core|.NET Core]]
- Named according to a "verb-noun" standard
	- `Get-Verb` returns all standard verbs
- `Get-Command` lists all available cmdlets
	- can be filtered with `-Noun` and/or `-Verb`