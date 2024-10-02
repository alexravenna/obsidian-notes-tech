---
tags:
  - cloud
  - cloud-agnostic
  - declarative
  - hashicorp
  - IaC
  - infrastructure
documentation:
  - https://developer.hashicorp.com/terraform/docs
from: "[[HashiCorp]]"
---
# Description
- [[Cloud-agnostic]] [[Infrastructure as Code]] tool
- Written in [[HCL]]
- Files describe the desired state of the infrastructure
- All `.tf` files in the execution folder are included
# Providers
- Written in [[Go]]
- Consist of:
	- resources
	- data sources

# Verify
- `terraform plan -out main.tfplan` outputs an execution plan without applying it
- If the plan is verified, apply it with `terraform apply main.tfplan`
# Clean up
- `terraform plan -destroy`

- locals
- .tfvars
- `terraform init`