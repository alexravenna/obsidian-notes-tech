---
aliases:
  - Dev containers
tags:
  - container
  - tool
homepage:
  - https://containers.dev/
specification: https://containers.dev/implementors/spec/
resources:
  - https://code.visualstudio.com/blogs/2022/09/15/dev-container-features
  - https://devblogs.microsoft.com/ise/dev-containers/
---
# Description
- A [[Virtualization/Containers/Docker/Docker|Docker]] [[Container Image|container image]] that contains all the tools and dependencies needed to run a development environment
- Defined in a `devcontainer.json` file, usually contained in the root directory or a .devcontainer directory
- Supported by [[IDE]]s such as:
	- [[Visual Studio Code|VS Code]]
	- [[IntelliJ]]
	- [[GitHub Codespaces]]
- IDE-specific properties and [[Environment Variables|environment variables]] can be defined
- Can base off of a remote base image or a local [[Dockerfile]]
- Lifecycle scripts can further customize the environment
## Features
- Docs: [Dev Container Features reference (containers.dev)](https://containers.dev/implementors/features/)
- Self-contained units of installation code
- Used for [[CLI]]s, dependencies and other tools
- All available official and community-supported features: [Features (containers.dev)](https://containers.dev/features)
- Contains at least:
	- `devcontainer-feature.json`: metadata about the feature
	- `install.sh`: an entrypoint script
## Templates
- Docs: [Dev Container Templates reference (containers.dev)](https://containers.dev/implementors/templates/)
- Source files packaged together
- Used for configuring a development environment
- - Contains at least:
	- `devcontainer-template.json`: metadata about the template
	- `.devcontainer.json`: an entrypoint script
- Packaged as [[tarballs]]
- Multiple templates can be stored in one "collection" with a `devcontainer-collection.json`
- #caveat Templates and features should be stored in separate [[Git]] [[Repository|repositories]]
## CLI
- Reference implementation: [devcontainers/cli: A reference implementation for the specification that can create and configure a dev container from a devcontainer.json. (github.com)](https://github.com/devcontainers/cli)

