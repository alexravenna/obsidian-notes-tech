---
created: 2024-05-21T10:18:23Z
updated: 2024-12-10T08:34:55Z
aliases:
  - Image
tags:
  - immutable
  - portable
  - virtualization
---
# Description
- Portable and immutable
- The unit of distribution for containerized applications
- A lightweight, isolated environment for building and running software
# Container Operating System
- Effectively the runtime environment for a containerized application
- An [[OS]] can be packaged into the image
	- For [[Linux]]-based images this isn't always necessary
	- For [[Windows]]-based images it is necessary
- The container OS is isolated from the host OS
# Image Types
- Base image
	- Builds upon the [[Virtualization/Containers/Docker/Docker|Docker]] `scratch` image, which is empty
	- `scratch` doesn't create a filesystem layer
	- Windows images always base upon a Windows base image
- Parent image
	- The image upon which you create your own images
	- Usually includes a container OS