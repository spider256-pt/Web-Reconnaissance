
#### Subdomains are important in web reconnaissance 

###### Reason:
1. Development and Staging Environment
2. Hidden Login Portals
3. Legacy Application
4. Sensitive information
Subdomain enumeration is the process of systematically identifying and listing these subdomains.

### Active Subdomain Enumeration

This involves directly interacting with the target domain's DNS servers to uncover subdomains. One method is attempting a `DNS zone transfer`, where a misconfigured server might inadvertently leak a complete list of subdomains

1. brute-force tools
	1. dnsenum
	2. ffuf
	3. gobuster

### Passive Subdomain Enumeration

This relies on external sources of information to discover subdomains without directly querying the target's DNS servers. One valuable resource is `Certificate Transparency (CT) logs`, public repositories of SSL/TLS certificates. These certificates often include a list of associated subdomains in their Subject Alternative Name (SAN) field, providing a treasure trove of potential targets.

[[DNS{Domain Name System}]]