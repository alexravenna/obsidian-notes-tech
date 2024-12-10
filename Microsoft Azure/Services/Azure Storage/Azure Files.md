---
created: 2024-04-23T08:26:05Z
updated: 2024-12-10T08:34:57Z
tags: []
---
- File shares
- Can be mounted concurrently by cloud or [[on-premise]] deployments
- Endpoint format: `https://<storage-account-name>.file.core.windows.net`
- Accessible via protocols:
	- [[SMB]] (on [[Windows]], [[Linux]] and [[macOS]] clients)
		- can be cached on [[Windows Server|Windows Servers]] with [[Azure File Sync]]
	- [[NFS]] (on Linux and macOS clients)