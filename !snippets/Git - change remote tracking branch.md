---
created: 2024-03-27T07:41:13Z
updated: 2024-12-10T08:33:15Z
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