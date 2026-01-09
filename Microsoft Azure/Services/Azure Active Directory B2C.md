---
created: 2023-11-13T10:59:49Z
updated: 2025-01-27T11:00:13+01:00
aliases:
  - AD B2C
tags:
  - "#authentication"
  - "#authorization"
  - azure
resources:
  - https://learn.microsoft.com/en-us/azure/active-directory-b2c/
  - https://www.youtube.com/watch?v=QuXI4rPaczc
---
# Description
- [[CIAM]] solution
- Is its own [[tenant]] and can't have any [[subscription|subscriptions]] associated with it
	- other [[Azure]] [[Resource|resources]] can't be created in this tenant
- Business-to-customer identity as a service
- Connection between identities (local, social, business, government) and business applications and APIs
- Supports:
	- [[OpenID Connect]]
	- [[OAuth]]
	- [[SAML]]
- Enables [[SSO]]
- Supports configurable, [[built-in]] user flows and custom policies
- User types:
	- Work
	- Guest
	- Consumer