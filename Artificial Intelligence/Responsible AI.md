---
tags:
  - ai
  - ethics
  - microsoft
resources:
  - https://learn.microsoft.com/en-us/azure/machine-learning/concept-responsible-ai
  - https://learn.microsoft.com/en-us/legal/cognitive-services/openai/overview
  - https://www.microsoft.com/en-us/ai/responsible-ai
---
- A term from [[Microsoft]]
- The principles and best practices to ensure that [[AI]] work are:
	- accountable
	- fair and inclusive
	- reliable and safe
	- transparent
	- secure
	- respects privacy
- Four stages in developing and implementing a responsible AI plan:
  1. Identify:
    1. Identify potential harms (such as generating offensive, inaccurate or illegal content)
    2. Prioritize identified harms
    3. Test and verify the prioritized harms
    4. Document and share the verified harms
  2. Measure:
    1. Measure potential harms with manual and automatic testing, such as using a classification model for "harmful" or "not harmful"
  3. Mitigate:
    1. Mitigate potential harms at four different layers:
      1. Model layer: maybe use a different model? Maybe [[fine-tune]] a [[Foundation Model|foundation model]]?
      2. Safety system layer: platform-level configurations like content filters, alert notifications
      3. Metaprompt and grounding layer:
        1. Specify metaprompts to define behavioral model parameters
        2. Add grounding data to input prompts to influence the output
      4. User experience layer:
        1. Constrain input and/or using input/output validation
        2. Be transparent in documentation about capabilities, limits and potential harms
  4. Operate:
    1. Complete prerelease reviewa
    2. Release with plans for:
      1. Phased delivery
      2. Incident response
      3. Rollbacks
    3. Implement capabilities for:
      1. User feedback and issue reporting
      2. Blocking users and IP addresses
      3. Blocking harmful responses upon discovering
      4. Tracking [[Observability/Telemetry|telemetry]] data
# Identify
- 