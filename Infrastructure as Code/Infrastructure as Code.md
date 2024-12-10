---
created: 2024-01-10T09:06:59Z
updated: 2024-12-10T08:34:59Z
aliases:
  - IaC
tags:
  - automation
  - cloud
  - configuration
  - infrastructure
training:
  - https://learn.microsoft.com/en-us/training/modules/terraform-introduction-to-infrastructure-as-code/
---
# Description
- The process of automating infrastructure [[provisioning]]
- Cloud infrastructure resources are defined in [[declarative]] code stored in a [[VCS]], just like application source code
- Cloud infrastructure is provisioned automatically by a tool that interprets this code
# Advantages
- Audit trail: through the changes in VCS you can track the history of updates
- Documentation: IaC code can function as infrastructure documentation
- Provisioning new environments can happen more quickly:
	- for non-production environments
	- as disaster recovery
- You can profit from existing code tooling:
	- [[linting]]
	- [[static code analysis]]
- [[idempotent|Idempotency]] helps avoid [[configuration drift]]