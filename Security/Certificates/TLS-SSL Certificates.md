---
aliases:
  - TLS/SSL Certificates
---

# Description
- Utilize the [[X.509]] format
- Issued by [[CA]]s
- Chained to a CAs root certificate
- The basis [[HTTPS]]
- Used to encrypt information transferred to and from a website/server
- Levels of validation, from lowest to highest, i.e. most anonymous to least anonymous:
	- Domain Validated (DV)
	- Organization Validated (OV)
	- Extended Validation (EV)
# SSL Handshake
-  Standard handshake for each new session:
	- Client hello
	- Server hello
	- Authentication: browser and server exchange and validate their respective certificates
	- Key exchange:
		- Server shares its [[Public Key Cryptography|public key]] with the browser
		- Browser uses public key to create and encrypt a pre-master key
	- Decryption: server decrypts the pre-master key with its [[Public Key Cryptography|private key]]
	- Encryption with session key: client and server exchange messages saying that future messages will be encrypted
		- This session key is [[Symmetric Encryption|symmetric]]