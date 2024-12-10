---
created: 2024-01-03T12:20:12Z
updated: 2024-12-10T08:34:59Z
tags:
  - ai
  - codex
  - copilot
  - github
  - openai
homepage:
  - https://github.com/features/copilot
documentation:
  - https://docs.github.com/en/copilot/about-github-copilot
resources:
  - https://github.blog/2023-05-17-inside-github-working-with-the-llms-behind-github-copilot/
  - https://github.blog/2023-06-20-how-to-write-better-prompts-for-github-copilot/
training:
  - https://learn.microsoft.com/en-us/training/modules/introduction-prompt-engineering-with-github-copilot/
  - https://learn.microsoft.com/en-us/training/paths/copilot/
---
# Description
- An AI [[pair programming|pair programmer]] from [[GitHub]]
- Powered by [[Codex]] 
- Supported [[IDE]]s:
	- [[Visual Studio]]
	- [[Visual Studio Code|VS Code]]
	- [[Neovim]]
	- [[JetBrains]] IDEs
- Steps behind a prompt:
  1. Prompt and context (nearby code, file type and name, open tabs) transmission (over [[HTTPS]])
  2. Content filtering to remove personal data and inappropriate content
  3. Intent extraction and mapping to understand and generate what concrete task Copilot should undertake
  4. Code generation
  5. User interaction (accept, modify or reject code suggestions)
  6. Copilot internal feedback loop
  7. Repeat for subsequent prompts
- GitHub Copilot for Business vs GitHub Copilot for Individuals:
	- [[VPN]] proxy support via [[Self-signed Certificate|self-signed certificates]]
	- zero data retention for snippets and telemetry
	- policy management organization-wide
- GitHub Copilot Enterprise features:
	- Copilot Chat is customized to the enterprise's codebase
	- [[PR]] summaries can be generated -> quickly create a PR description for reviewers
	- Docsets management:
		- Docsets are private collections of internal code and documentation
			- You can add GitHub [[Repository|repos]] and specific files from repos to be indexed
		- Copilot can answer questions using these docsets
	- Copilot code reviews