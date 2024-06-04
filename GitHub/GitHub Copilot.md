---
tags:
  - ai
  - codex
  - copilot
  - github
  - openai
resources:
  - https://github.blog/2023-05-17-inside-github-working-with-the-llms-behind-github-copilot/
  - https://github.blog/2023-06-20-how-to-write-better-prompts-for-github-copilot/
training:
  - https://learn.microsoft.com/en-us/training/modules/introduction-prompt-engineering-with-github-copilot/
---
# Description
- An AI [[pair programming|pair programmer]] from [[GitHub]]
- Powered by [[Codex]] 
- Steps behind a prompt:
  1. Prompt and context (nearby code, file type and name, open tabs) transmission (over [[HTTPS]])
  2. Content filtering to remove personal data and inappropriate content
  3. Intent extraction and mapping to understand and generate what concrete task Copilot should undertake
  4. Code generation
  5. User interaction (accept, modify or reject code suggestions)
  6. Copilot internal feedback loop
  7. Repeat for subsequent prompts