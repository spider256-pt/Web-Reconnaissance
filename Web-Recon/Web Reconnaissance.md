
1. Web Reconnaissance is the foundation of the security assessment.
2. This involves collecting information about target website or targets web application.
3. This is a preparatory phase before diving into deeper analysis and potential exploitation.
4. The "Information Gathering" phase of the Penetration Testing Process.
## Primary Goals of Web reconnaissance:

- ***Identifying Assets***: publicly accessible components of the target.{webpages, subdomains and etc.}

- ***Discovering Hidden Information***: locating sensitive data might be inadvertently{backup files, configuration files, etc}

- ***Analyzing the Attack Surface***: Examine the targets attack  surface to identify potential vulnerabilities and weakness. {technologies used, machine version and points for exploitation}

- ***Gathering Intelligence***: Gathering the information that can be leveraged for further exploitation or social engineering attacks.

## Types of Reconnaissance:

1. Active 
2. Passive

#### 1. Active Reconnaissance:

In active Reconnaissance, the attacker directly interacts with the target system.

1. Port scanning | ***==Tools==*** ***==|==*** nmap, Masscan, Unicornscan | ***==Risk==*** | High |

2. Vulnerability Scanning | ***==Tools==*** | OpenVAS, Nikto, Nessuss | ***==Risk==*** | High |

3. Network Mapping | ***==Tools==*** | Traceroute, Nmap | ***==Risk==*** | Medium

4. Banner Grabbing | ***==Tools==*** | Netcat, curl | ***==Risk==*** | Low

5. Os Fingerprinting | ***==Tools==*** | Nmap, Xprobe2 | Risk | Low

6. Service Enumeration | ***==Tools==*** | Nmap | ***==Risk==*** | Low

7. Web spidering | ***==Tools==*** |Burp suite spider, OWASP ZAP spider,etc. | ***==Risk==*** | Low to Medium

#### 2. Passive Reconnaissance:

In passive Reconnaissance the attacker gather information without any direct interaction.

1. Search Engines Queries | ***==Tools==*** | Google, DuckDuckGo,etc | ***==Risks==*** | very low

2. WHOIS lookups | ***==Tools==*** | Whois Command Cli based | ***==Risks==*** | very low

3. DNS | ***==Tools==*** | dig, nslookup, host, dnsenum, etc | ***==Risks==*** | very low
4. Web Archive Analysis | ***==Tools==*** | Wayback Machine | ***==Risks==*** | very low

5. Social Media Analysis | ***==Tools==*** | LinkDin, Twitter, Facebook, etc | ***==Risks==*** | very ***==low==***

6. Code Repositories | ***==Tools==*** | GitHub, GitLab | ***==Risks==*** | very low