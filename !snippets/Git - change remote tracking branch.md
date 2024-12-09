---
tags:
  - git
  - snippet
resources:
  - https://stackoverflow.com/questions/4878249/how-to-change-the-remote-a-branch-is-tracking
---
- E.g. after renaming a local branch that is already tracked remotely:
	- Rename local branch
	- Delete remote branch
	- Change tracking branch for remote branch
- `git branch <branch_name> --set-upstream-to <remote_name>/<new_branch_name>`