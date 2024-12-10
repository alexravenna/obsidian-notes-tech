---
created: 2024-05-21T11:43:56Z
updated: 2024-12-10T08:34:54Z
documentation:
  - https://docs.docker.com/engine/network/drivers/host/
---

- Bridge network ([[Linux]]) or NAT network ([[Windows]])
	- Default network configuration
	- Container ports can be mapped to host ports with e.g. `--publish 8080:80`
- Host network
	- Not available under Windows or [[macOS]]
	- Supported under [[Docker Desktop]] for Linux containers
- None network
	- Networking is disabled