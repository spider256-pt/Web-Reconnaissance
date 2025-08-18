1. Fingerprinting focuses on extracting technical details about the technologies powering a website or a web-application.

Fingerprinting servers as a cornerstone of web reconnaissance for several reasons:

1. Targeted Attacks
2. Identifying Misconfiguration
3. Prioritising Targets
4. Building Comprehensive Profile

## Fingerprinting Techniques

- `Banner Grabbing`: Often reveals server software, version number, and other details.

- `Analyzing HTTP Headers`: The `Server` header typically discloses the web server software, while the `X-Powered-By` header might reveal additional technologies like scripting languages or frameworks.

- `Probing for Specific Response`:  Sending specially crafted requests to the target can elicit unique responses that reveal specific technologies or versions, error messages or behaviors. 

- `Analyze Page Content`: A web page's content, including its structure, scripts, and other elements, can often provide clues about the underlying technologies


## Most Used Tools


| Tool       | Features                                                                                          |
| ---------- | ------------------------------------------------------------------------------------------------- |
| Wappalyzer | Identifies a wide range of web technologies, including CMS, framework, analytics tools and more   |
| Builtwith  | Detailed reports on websites technologies                                                         |
| WhatWeb    | CLI tool for website fingerprinting                                                               |
| Nmap       | Can be used with NSE for fingerprinting                                                           |
| Netcraft   | Offers a range of web security services, including website fingerprinting and security reporting. |
| wafw00f    | Command-line tool specifically designed for identifying Web Application Firewalls (WAFs)          |

###### Footprinting steps:


1. Banner grabing:

	`curl -I <Domain_name>`

	curl commands with the `-I flag or --head` to fetch only for HTTP headers

2. For detection of WAF{Web Application Firewall} 

	`wadw00f <Domain_name>`

	Is used to detect web application firewall.
	
3. For vulnerability assessment

	`nikto -h <domain_name> -Tuning b`

	`-h`  specifies  target<host>
	
	-Tuning b tells Nikto to only run the Software identification module.

for more information use man tool for each one of them.

	``man <tool>``