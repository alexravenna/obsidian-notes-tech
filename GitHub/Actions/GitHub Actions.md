---
tags:
  - automation
  - ci-cd
  - pipeline
documentation:
  - https://docs.github.com/en/actions
training:
  - https://learn.microsoft.com/en-us/training/modules/introduction-to-github-actions/
---
# Description
- Enable [[CI]]/[[CD]] workflows in [[GitHub]]
- Can also be used for automating a wide variety of other GitHub tasks
- Defined in [[YAML]]
- Executed on runners
	- Either hosted by GitHub or [[self-hosted]]
- Can be defined locally in a [[Repository|repo]] or contributed to and consumed from the [Marketplace (github.com)](https://github.com/marketplace?type=actions)
- Types:
	- Docker
	- JavaScript
	- Composite
- Flow: [[Actions flow.canvas|Actions flow]]
- Events types:
	- scheduled ([[cron]]-based)
	- code events, e.g. upon [[pull|pulling]] or opening a [[PR]]
	- manual (only if workflow on the [[default branch]])
	- GitHub [[Webhooks|webhooks]] (usually only if workflow on the default branch]])
- Workflows:
	- found in `.github/workflows`
	- can be manually triggered
	- defines the automation:
		- events and triggers
		- jobs to run when triggered
		- where to run the jobs, i.e. with which runner
# Workflow Syntax
- `on`: defines triggering event
- `jobs`: list of jobs to execute
- Job:
	- `runs-on`: which runner to execute on
	- `steps`: a list of steps to execute
		- `uses`: which Action to consume