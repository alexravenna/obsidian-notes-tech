---
tags:
  - cloud
  - cloud-agnostic
  - declarative
  - hashicorp
  - IaC
  - infrastructure
---
# Description
- [[Cloud-agnostic]] [[Infrastructure as Code]] tool
- Written in [[HCL]]
- Files describe the desired state of the infrastructure
- All `.tf` files in the execution folder are included
# Providers
## For Azure
- AzureRM: Manage [[Azure Resource Manager|ARM]] resources
- AzureAD: Manage [[Microsoft Entra]] resources
- AzureDevOps: Manage [[Azure DevOps]] resources
- AzAPI: Manage Azure [[Resource|resources]] by using the ARM APIs directly
- Azure Stack: Manage [[Azure Stack]] resources
# Verify
- `terraform plan -out main.tfplan` outputs an execution plan without applying it
- If the plan is verified, apply it with `terraform apply main.tfplan`
# Clean up
- `terraform plan -destroy`

- locals
- .tfvars
- `terraform init`