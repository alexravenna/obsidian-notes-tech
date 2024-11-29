---
tags:
  - authorization
  - security
resources:
  - https://developer.okta.com/blog/2019/10/21/illustrated-guide-to-oauth-and-oidc
  - https://fusionauth.io/articles/oauth/modern-guide-to-oauth
  - https://www.youtube.com/watch?v=t18YB3xDfXI
  - https://www.youtube.com/watch?v=ZV5yTm4pT8g
---
# Description
- An [[Security/Authorization|authorization]] [[protocol]] that allows a [[third-party]] app to access web resources for a user
- Resources have an identifier: application ID [[URI]]
- Scopes: types of permission sets
	- Requested with the `scope` [[query parameter]]
- Permissions are strings appended to application ID URIs
- Flows:
	- authorization code
# Terminology
- Resource owner: you
- client
- authorization server
- resource server
- redirect URI/callback URL
- response type
- scope: granular permissions the client wants
- consent
- client ID/app ID
- client secret/app secret
- authorization code
- access token: used by client for communication with resource server