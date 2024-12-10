---
created: 2024-03-06T17:29:02Z
updated: 2024-12-10T08:34:59Z
tags:
  - automation
  - ci-cd
  - pipeline
documentation:
  - https://docs.github.com/en/actions
resources:
  - https://github.com/actions/starter-workflows
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
- Jobs:
	- can be dependent on one another
	- if not, they run in parallel
	- all steps in one job execute on the same runner and share the same filesystem
- Runners:
	- self-hosted runners:
		- have to be registered before use
		- can be added at repo, organization and enterprise level
- Versions:
	- the latest version of an Action is always automatically retrieved
	- you can specify a specific version through:
		- tags: `-uses: actions/install-timer@v2.0.1`
		- [[SHA]]-based hashes: `-uses: actions/install-timer@327239021...`
		- the latest version from a specific branch: `-uses: actions/install-timer@develop`
# Workflow Syntax
- `on`: defines triggering event
- `jobs`: list of jobs to execute
- Job:
	- `runs-on`: which runner to execute on
	- `steps`: a list of steps to execute
		- `uses`: which Action to consume
# Environment Variables
- All built-in [[Environment Variables|environment variables]] have the `GITHUB_` prefix
- Examples:
	- `GITHUB_WORKFLOW`: the name of the workflow
	- `GITHUB_ACTION`: the unique identifier for the action
	- `GITHUB_REPOSITORY`: owner/repo
- Passed in with the `env:` key