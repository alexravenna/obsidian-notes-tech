---
created: 2024-01-04T16:03:06Z
updated: 2024-12-10T08:34:59Z
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
# Workflow
- `init`
	- initializes working directory and downloads provider plugins and modules
- `plan`
	- creates an execution plan
- `apply`
	- applies the execution plan (implicitly runs `plan` first if no plan provided)
- `destroy`
	- deletes infrastructure managed by Terraform
	- alias of `apply -delete`
# Taint
- `tf taint`
# Backend
- Cannot access variables because it is used before variable resolution
- Changes to backend configuration requires re-initialization

# Formatting
- `tf fmt`