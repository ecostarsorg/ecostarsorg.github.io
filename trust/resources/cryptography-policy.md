# Cryptography policy
* Version: v1.1
* Date of version: 2024-04
* Author: Information Security Officer
* Approver: CTO
* Confidentiality: Internal use. Shared upon request as part of a due diligence

## Data encryption 
### Data in-transit
* Type: 
* Algorithm: TLS 1.2+ (using a subset of ciphers considered secure)
* Provider: [Let’s Encrypt](https://letsencrypt.org/) and tied to the domain name. 

### Data at-rest
* Type: encryption at disk level
* Algorithm: AES
* Key length: 256

### Passwords and secrets
* Type: hash
* Algorithm: Argon2id
* Key length: 256 bit

### Tokens
* Type: hash
* Algorithm: SHA
* Key length: 256

### Laptop disks
* Type: encryption
* Algorithm: AES 
* Key length: 256 or 528 bit

### Web certificate
* Type: digital signature
* Algorithm: 
* Key length: 

### Web cypher
* Type: AES
* Algorithm: 
* Key length: 

