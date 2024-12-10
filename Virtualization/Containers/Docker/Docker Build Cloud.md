---
created: 2024-02-05T11:45:27Z
updated: 2024-12-10T08:34:55Z
aliases:
  - DBC
tags:
  - build
  - cloud
  - docker
homepage:
  - https://www.docker.com/products/build-cloud/
documentation:
  - https://docs.docker.com/build/cloud/
---
# Description
- A service offered by [[Virtualization/Containers/Docker/Docker|Docker]] for off-loading the building of container images to a dedicated, remote [[BuildKit]] instance
- Features promising speed increases:
	- Build processes don't slow down/block developer machines
	- Parallel builds are possible (depending on the user plan)
	- Native builders for [[AMD]] and [[ARM Architecture|ARM]] architectures 
	- Cache sharing amongst developer team members