---
created: 2024-06-12T09:01:37Z
updated: 2024-12-10T08:34:57Z
documentation:
  - https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/nslookup
---
# Description
- Example: `nslookup`
	- answers with default [[DNS]] [[Name Server|name server]]
	- goes into interactive mode
- Example: `nslookup mydomain.com 1.1.1.1
	- look up the IP of `mydomain.com` using the name server `1.1.1.1`
- Authoritative answer: from an official (i.e. authoritative) name server
- Non-authoritative answer: from any other name server
- [domain name system - DNS - NSLOOKUP what is the meaning of the non-authoritative answer? - Server Fault](https://serverfault.com/questions/413124/dns-nslookup-what-is-the-meaning-of-the-non-authoritative-answer)