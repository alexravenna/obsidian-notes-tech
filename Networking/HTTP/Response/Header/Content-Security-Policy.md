---
created: 2024-08-28T07:38:41Z
updated: 2024-12-10T08:34:57Z
aliases:
  - CSP
specification: "[[Content Security Policy Level 2]]"
resources:
  - https://cheatsheetseries.owasp.org/cheatsheets/Content_Security_Policy_Cheat_Sheet.html
  - https://content-security-policy.com/
---
# Description
- Restricts which resources can be loaded into a web page and the [[URL]]s that they can come from
- Can be set on the server or as a [[meta]] tag
- Has multiple directives for different resource types
- Some directives can be extended with source lists that allow more granular restrictions
# Examples
- Only accept resources from the same origin:
  `Content-Security-Policy: default-src 'self'`