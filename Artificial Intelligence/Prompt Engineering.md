---
created: 2024-02-09T09:14:01Z
updated: 2024-12-10T08:35:01Z
aliases:
  - Prompt Design
resources:
  - https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/prompt-engineering
  - https://learn.microsoft.com/en-us/training/modules/introduction-prompt-engineering-with-github-copilot/
training:
  - https://learn.microsoft.com/en-us/training/modules/create-prompts-for-generative-ai-training-tools/
---
# Description
- The process of creating a [[Prompt|prompt]] that guide the [[AI]] system to generate the desired output
# Principles
- 4 S's:
	- Single: ask the AI a single, well-defined question or to do a single, well-defined task
	- Specific: use explicit and detailed instructions
	- Short: keep prompts concise and to the point
	  Surround: provide context (e.g. keep related files open)
# Practices
- Zero-shot learning:
	- When the AI generates a result with one prompt simply by using its training to date
- One-shot learning:
	- When the AI generates a result after a single example is given
- Few-shot learning:
	- When the AI generates a result after being presented with multiple examples