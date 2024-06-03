---
tags:
  - umbraco
resources:
  - https://our.umbraco.com/documentation/Add-ons/Umbraco-Deploy/
---
- Two separate parts of deployment:
	- meta data (document types, templates, etc.) -> AKA deploy
	- content (content nodes and media) -> AKA transfer
- Meta data is stored in a repository and deployed with a CI/CD pipeline
- Content and media are not stored in a repository: they are transferred directly from the Umbraco backoffice 