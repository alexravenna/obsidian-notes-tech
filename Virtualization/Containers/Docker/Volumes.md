# Description
- A volume is stored on the host filesystem
- Created with `docker volume create`
- Can also be defined in a [[Dockerfile]]
- [[Docker]] mounts and manages volumes
- They are isolated from the host machine
- Aren't automatically removed when no longer used
- Preferred over [[Bind mounts|bind mounts]]