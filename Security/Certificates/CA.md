---
created: 2024-03-01T09:30:42Z
updated: 2024-12-10T08:34:56Z
aliases:
  - Certificate Authority
---
# Description
- Part of [[PKI]]
- A trusted organization that issues [[TLS-SSL Certificates|TLS/SSL Certificates]] for websites and other entities
- The applicant has their identity verified before being issued a certificate
- CAs possess a root certificate
	- This is pre-downloaded in most browsers
- Encrypts [[hash|hashed]] information in certificate with [[private key]]
- Public key is available in browser - can be used to decrypt [[certificate]]
- Digital signature