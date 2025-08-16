
## DNS Tools

DNS reconnaissance involves utilizing specialized tools to extract valuable information from DNS servers.

| Tool                       | Key features                                                                                                                   |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| dig                        | supports various query types (A,MX,NS,TXT, etc)                                                                                |
| nslookup                   | Simpler DNS lookup, A, AAAA and MX records                                                                                     |
| host                       | Quick checks of A,AAAA and MX records                                                                                          |
| dnsenum                    | Dns enumeration, dictionary attacks, brute-forcing, zone-transfer(if allowed).                                                 |
| fierce                     | Dns reconnaissance, sub-domain enum, recursive search and wild-card detection.                                                 |
| dnsrecon                   | Combines multiple DNS reconnaissance techniques and supports various output formats.                                           |
| theHarvester               | An OSINT tool collecting email addresses, employee information, and other data associated with a domain from multiple sources. |
| Online DNS Lookup Services | User-friendly interfaces for performing DNS lookups                                                                            |

##### dig(domain information groper)

###### Commands:


1. dig @1.1.1.1 domain.com | specifies name sever to query; in this case 1.1.1.1
2. dig +trace domain.com | shows the full path to the query.
3. dig +short domain.com | Provides a short answer to the query.
4. dig +noall +answer domain.com | display only the answer section of the query output.
5. dig domain.com ANY | Retrieves all available DNS records for the domain.


[[DNS{Domain Name System}]]


  