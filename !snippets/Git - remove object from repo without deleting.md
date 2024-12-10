---
created: 2023-11-22T09:04:03Z
updated: 2024-12-10T08:33:15Z
tags:
  - git
  - snippet
resources:
  - https://stackoverflow.com/questions/1274057/how-do-i-make-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitignore
---
Remove file/folder (recursively) that was tracked up until now and should remain in your working copy: 
`git rm -r --cached path/to/file`