---
created: 2024-05-21T11:36:20Z
updated: 2024-12-10T08:34:54Z
---
# Description
- A volume is stored on the host filesystem
- Created with `docker volume create`
- Can also be defined in a [[Dockerfile]]
- [[Virtualization/Containers/Docker/Docker|Docker]] mounts and manages volumes
- They are isolated from the host machine
- Aren't automatically removed when no longer used
- Preferred over [[Bind mounts|bind mounts]]