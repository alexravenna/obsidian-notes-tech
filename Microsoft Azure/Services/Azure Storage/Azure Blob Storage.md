---
created: 2023-11-29T15:30:43Z
updated: 2024-12-10T08:34:57Z
tags:
  - azure
  - blob
  - storage
---
# Description
- Object storage solution
- For unstructured data (text, binary)
- Endpoint format: `https://<storage-account-name>.blob.core.windows.net`
# Blob Types
- Block blobs
	- 
- Append blobs
	- Optimized for append operations
	- Useful for things like logs, where existing blobs have to be appended to
- Page blobs
	- Optimized for random read and write operations