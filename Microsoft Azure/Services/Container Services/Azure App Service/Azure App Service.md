---
aliases:
  - APS
  - Azure Web Apps
  - Azure Web Sites
tags:
  - azure
  - PaaS
documentation:
  - https://learn.microsoft.com/en-us/azure/app-service/
training:
  - https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-app-service/
  - https://learn.microsoft.com/en-us/training/paths/create-azure-app-service-web-apps/
---
# Description
- [[PaaS]] offering for hosting web apps, [[REST|REST API]]s and mobile back ends
- Built-in scalability:
	- up/down: more/less [[CPU]] and/or [[RAM]]
	- in/out: more/fewer instances running the web app
- Allows auto-syncing code with:
	- [[Azure DevOps]] (automated)
	- [[GitHub]] (automated)
	- [[Bitbucket]] (automated)
	- [[FTP]] (manual)
	- [[Azure CLI]] (manual): `az webapp up`
	- a local [[Git]] repository pushed to the App Service (manual)
	- zip file sent by HTTP to the App Service (manual)
- App Service on Linux:
	- Many built-in images available for common language/framework runtimes
	- Web App for Containers: the ability to run custom [[Linux]] [[Container Image|containers]]
- Deployment slots enable different environments, such as staging and production
- Code is built by [[Oryx]]
# Plans
- An app always runs in an App Service plan
- Defines a set of compute resources
- One or more apps can run on the same resources
- Characteristics:
	- [[OS]]
	- region
	- number and size of [[VM]] instances
	- pricing tier
		- Free and Shared don't scale and share resources with other apps
- All apps (one or more) in the same plan share the same VM instances

# Authentication and Authorization
- Built-in
- Uses [[federated identity]] through third-party [[Identity Provider|identity providers]]
- Default identity providers (any number can be used):
	- Microsoft identity platform
	- Facebook
	- Google
	- Twitter
	- Any [[OpenID Connect]] provider
	- GitHub
- The authentication and authorization module runs separately from app code and can be configured without code