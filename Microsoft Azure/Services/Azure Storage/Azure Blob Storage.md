---
created: 2023-11-29T15:30:43Z
updated: 2025-04-10T13:55:13+02:00
tags:
  - azure
  - blob
  - storage
---
# Description
- An object storage solution
- For [[unstructured data]] (text, binary)
- Endpoint format: `https://<storage-account-name>.blob.core.windows.net`
- Containers are the next level of blob organization:
	- `https://<storage-account-name>.blob.core.windows.net/<container-name>`
- Accessible via:
	- the [[Azure Storage]] [[REST]] [[API]]
	- [[Azure PowerShell]]
	- [[Azure CLI]]
	- an [[Azure Storage]] client library
# Blob Types
- Block blobs
	- store text and [[binary]] data
- Append blobs
	- Optimized for append operations
	- Useful for things like logs, where existing blobs have to be appended to
- Page blobs
	- Optimized for random read and write operations
	- store [[VHD]] files, e.g. [[Azure Disk Storage]]
- 