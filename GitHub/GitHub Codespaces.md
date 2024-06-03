---
tags:
  - CDE
  - container
  - github
homepage:
  - https://github.com/features/codespaces
documentation:
  - https://docs.github.com/en/codespaces
resources:
  - https://learn.microsoft.com/en-us/training/modules/code-with-github-codespaces/
---
# Description
- A [[Cloud Development Environment|CDE]] from [[GitHub]]
- Each Codespace is a [[Container|container]] on a Linux [[Virtual Machine|VM]] in the [[Microsoft Azure/Azure]] cloud
- You can create a Codespace:
	- on [GitHub](github.com)
	- in [[Visual Studio Code|VS Code]]
	- with the [[GitHub CLI]]
	- while editing on [[GitHub.dev]]
- Multiple Codespaces running at the same time are possible per [[repo]] and per [[Branch]]
- Number of total Codespaces is limited per user according to your subscription
- Prebuilds are possible for speeding up Codespace creation
- All work (including the clone of the repo) is stored under `/workspace`
# Lifecycle
- Codespaces be used for temporary work or for long-running development
- You can disconnect from and reconnect to a running Codespace at any time
- You can stop and restart Codespaces without losing changes
- A Codespace is stopped:
	- actively
	- after a period of 30 minutes (default):
		- after closing the connection (e.g. by closing the browser tab)
		- after inactivity
- Codespaces can be rebuilt:
	- Can be done to implement changes to the dev container configuration
	- An alternative is to create a new Codespace
	- A normal rebuild uses cached images; a full rebuild clears and cache and uses fresh images
	- Changes
		- outside of `/workspace` are cleared
		- inside of `/workspace` are preserved
- Stopped and inactive Codespaces are automatically deleted after 30 (which is configurable)
# Customization
- Codespaces are configurable with [[Development Containers|dev containers]]
- A [[dotfiles]] repository can be used to bootstrap the Codespace
- Settings Sync from [[Visual Studio Code|VS Code]] can be used
- [[Visual Studio Code|VS Code]] extensions or [[JetBrains]] plugins can be added to a Codespace
- The resources (i.e. [[CPU]]s) used by the Codespace can be adjusted
