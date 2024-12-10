---
created: 2023-11-15T10:23:42Z
updated: 2024-12-10T08:35:01Z
tags:
  - azure-devops
  - ci-cd
  - devops
documentation:
  - https://learn.microsoft.com/en-us/azure/devops/pipelines/
---
# Description
- A [[CI]]/[[CD]] service from [[Azure DevOps]]
- Provides infrastructure for automated [[Pipelines|pipelines]] to run on
- Integrates with various [[VCS]]:
	- [[GitHub]] 
	- [[GitLab]]
	- [[Azure Repos]]
	- [[Bitbucket]]
	  [[Subversion]]
- Terms:
	- Deployment target: where an application will be deployed to and hosted on
	- Job: a collection of steps to be run during a build
	- Pipeline: the process definition for CI/CD; consists of tasks
	- Stage: primary divisions of a pipeline
	- Task: the building block of a pipeline
	- Trigger: when a pipeline should run
- Agents:
	- can be [[self-hosted]] under:
		- [[Windows]]
		- [[macOS]]
		- [[Linux]]
		- [[Virtualization/Containers/Docker/Docker|Docker]]
	- or hosted by [[Microsoft/Microsoft|Microsoft]]
# Tasks
- [[Azure App Service Deploy]]
- [[IIS WebApp Deploy]]
