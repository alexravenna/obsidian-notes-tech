---
documentation:
  - https://learn.microsoft.com/en-us/entra/identity-platform/
resources:
  - https://www.youtube.com/playlist?list=PL3ZTgFEc7LyvP6Jo4kfgEjzgi7UdnzR-t
training:
  - https://learn.microsoft.com/en-us/training/modules/explore-microsoft-identity-platform/
---
# Description
- Components:
	- [[Authentication|authentication]] service:
		- compliant with [[OAuth 2.0]] and [[OpenID Connect]] standards
		- authenticates different identity types:
			- work or school accounts with [[Microsoft Entra ID]]
			- [[Microsoft]] accounts
			- social or local accounts with [[Azure Active Directory B2C]]
			- social or local customer accounts with [[Microsoft Entra External ID]]
	- open-source libraries like [[MSAL]]
	- Microsoft identity platform [[endpoint]] that works with MSAL and other libraries
	- application management portal
	- application configuration [[API]] through [[Microsoft Graph API]] and [[PowerShell]]
- Integrates:
	- [[passwordless]] authentication
	- step-up authentication
	- conditional access
- Two supported permission types:
	- delegated access
		- for apps that have a signed-in user; app acts as delegate for user
		- A user or administrator can consent to the permission requests
	- app-only access
		- for e.g. background services or [[daemon|daemons]] where no user is signed-in
		- only an administrator can consent to the permission requests
- Conditional Access enables:
	- [[MFA]]
	- allowing access only to [[Intune]]-enrolled devices
	- restricting user locations and [[IP Address|IP]] ranges
# Consent
- Types:
	- static user consent
	- incremental and dynamic user consent
	- admin [[CD]]
