
1. Subdomain Brute-Force Enumeration is a powerful active subdomain discovery technique that leverages pre-defined lists of potential subdomain names.
2. This approach systematically tests these names against the target domain to identify valid subdomains.
#### The process breaks down into four steps:

1. Wordlists selection
2. Iteration and querying
3. DNS Lookup
4. Filtering and validation

### DNSEnum

dnsenum is a widely-used cli tool written in perl. It is a comprehensive toolkit for:

1. DNS Record Enumeration
2. Zone Transfer Attempts
3. SubDomain Brute-Forcing 
4. google Scrapping
5. Reverse Lookup
6. WHOIS lookup

For more info about the tool use `man dnsenum` and wordlist from `Seclists`

`-f` for brute-forcing after choosing thee wordlist.
`-r` for recursive subdomain brute-forcing 

###### command

1. dnsenum --enum <domain-name> -f <path/wordlists> -r {for recursive}
2.  dnsenum --enum <domain-name> -f <path/wordlist>