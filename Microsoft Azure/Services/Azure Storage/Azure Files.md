---
created: 2025-04-10T13:39:07+02:00
updated: 2025-04-10T13:39:12+02:00
tags:
---
# Description
- File shares
- Can be mounted concurrently by cloud or [[on-premise]] deployments
- Endpoint format: `https://<storage-account-name>.file.core.windows.net`
- Accessible via protocols:
	- [[SMB]] (on [[Windows]], [[Linux]] and [[macOS]] clients)
		- can be cached on [[Windows Server|Windows Servers]] with [[Azure File Sync]]
	- [[NFS]] (on Linux and macOS clients)