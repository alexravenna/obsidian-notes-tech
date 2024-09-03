# Description
- System-assigned
	- Lifecycle is tied to the creating [[Resource|resource]]
- User-assigned
	- Can be used on multiple resources
	- A special [[Service Principal|service principal]] is created in [[Entra ID]]
	- The managed identity is authorized to have access to one or more services
	- Can be created:
		- in the [[Azure portal]]
		- with the [[Azure CLI]]: `az identity create -g RG1 -n uami-apl2003`