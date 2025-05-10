---
created: 2023-11-16T09:23:53Z
updated: 2025-05-10T11:59:12+02:00
aliases:
  - APS
  - Azure Web Apps
  - Azure Web Sites
tags:
  - azure
  - PaaS
  - application-hosting
documentation:
  - https://learn.microsoft.com/en-us/azure/app-service/
training:
  - https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-app-service/
  - https://learn.microsoft.com/en-us/training/paths/create-azure-app-service-web-apps/
---
# Description
- Supports [[Windows]] and [[Linux]] environments
- [[PaaS]] offering for hosting web apps, [[REST|REST API]]s and mobile back ends
- Built-in scalability:
	- up/down: more/less [[CPU]] and/or [[RAM]]
	- in/out: more/fewer instances running the web app
- Supports multiple languages/frameworks:
	- [[NET|.NET]]
	- [[NET Core|.NET Core]]
	- [[Java]]
	- [[Ruby]]
	- [[Node.js]]
	- [[PHP]]
	- [[Python]]
- Allows auto-syncing code ([[CD|continuous deployment]]) with:
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
# Types
## Web Apps
- Supports:
	- [[ASP.NET]]
	- [[ASP.NET Core]]
	- [[Java]]
	- [[Ruby]]
	- [[Node.js]]
	- [[PHP]]
	- [[Python]]
- Possible host systems:
	- [[Windows]]
	- [[Linux]]
## API Apps
- Offers full [[Swagger]] support
- [[API]]s can be packaged and published to the [[Azure Marketplace]]
- Apps can be consumed by [[HTTP]] or [[HTTPS]] clients
## WebJobs
- See [[Azure App Service WebJobs]]

## Mobile Apps
- Used for building [[backend]]s for mobile apps
- Offers functionality for:
	- storing data in [[Azure SQL Database]]
	- [[authentication]] against social [[Identity Provider|providers]]:
		- [[MSA]]
		- [[Google/Google|Google]]
		- [[X]]
		- [[Facebook]]
	- sending [[push notifications]]
	- running custom [[Csharp|C#]] or [[Node.js]] backend code
- Provides SDKs for mobile apps using:
	- native [[iOS]]
	- native [[Android]]
	- [[React Native]]
	- [[Xamarin]]