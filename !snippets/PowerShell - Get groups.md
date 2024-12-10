---
created: 2023-11-20T08:51:51Z
updated: 2024-12-10T08:33:15Z
tags:
  - powershell
  - RSoP
  - snippet
---
Show the Resultant Set of Policy (RSoP) info for the current user:
`gpresult /r /scope:user`

Show the Resultant Set of Policy (RSoP) info for the computer (needs admin rights):
`gpresult /r /scope:computer`