---
tags:
  - git
  - snippet
resources:
  - https://stackoverflow.com/questions/1274057/how-do-i-make-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitignore
---
Remove file/folder (recursively) that was tracked up until now and should remain in your working copy: 
`git rm -r --cached path/to/file`