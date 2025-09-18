---
created: 2025-09-16T09:54:49+02:00
updated: 2024-12-10T12:57:41Z
aliases:
  - JSON Web Token
---
# Description
- Three parts:
	- header
	- payload/body
	- signature
- Claims inside payload/body:
	- `sub`: subject - unique identifier for a user
	- `name`
	- `preferred_username`
	- `oid`: object ID
	- `tid`: tenant ID
	- `aud` - intended receiver
	- `iss` - [[Identity Provider]] who created it