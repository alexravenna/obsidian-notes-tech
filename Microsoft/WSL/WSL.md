---
aliases:
  - Windows Subsystem for Linux
documentation:
  - https://learn.microsoft.com/en-us/windows/wsl/
training:
  - https://learn.microsoft.com/en-us/training/modules/wsl-introduction/
---
- #caveat Automatically gives file access to Windows files and paths
- Files are viewable in Windows Explorer under `\\wsl.localhost\<distribution_name>`
- Utilized by [[Docker Desktop]]
- Set the default distribution: `wsl --set-default <Distribution Name>`
- Enter the Bash command line from PowerShell: `wsl ~`