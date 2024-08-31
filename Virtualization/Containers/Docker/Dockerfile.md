---
tags:
  - file-format
  - text
---
# Description
- A text-based file format that contains the instructions for building and running a [[Docker image]]
# Components
- [[Container Image#Image Types|Base or parent image]] we are building upon
- Commands: `CMD`
- Artifacts (files, etc.) to include/copy into the image: `COPY`or `INCLUDE`
- [[Network ports]] to be exposed to the host: `EXPOSE`
- Which command to run upon running the container: `ENTRYPOINT`