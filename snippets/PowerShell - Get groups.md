---
tags:
  - powershell
  - snippet
  - RSoP
---
Show the Resultant Set of Policy (RSoP) info for the current user:
`gpresult /r /scope:user`

Show the Resultant Set of Policy (RSoP) info for the computer (needs admin rights):
`gpresult /r /scope:computer`