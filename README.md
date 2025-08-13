# Web Reconnaissance – Foundation of Security Assessment

Web Reconnaissance is the foundation of any security assessment.  
It involves collecting information about a target website or web application, acting as a **preparatory phase** before deeper analysis and potential exploitation.  
This is also known as the **"Information Gathering" phase** in the Penetration Testing Process.

---

## 🎯 Primary Goals of Web Reconnaissance

- **Identifying Assets**  
  Discover publicly accessible components of the target such as webpages, subdomains, etc.

- **Discovering Hidden Information**  
  Locate sensitive data that might be inadvertently exposed (backup files, configuration files, etc.).

- **Analyzing the Attack Surface**  
  Examine the target's attack surface to identify potential vulnerabilities and weaknesses (e.g., technologies used, machine version, exploitable points).

- **Gathering Intelligence**  
  Collect information that can be leveraged for further exploitation or social engineering attacks.

---

## 🛠 Types of Reconnaissance

1. **Active Reconnaissance**  
2. **Passive Reconnaissance**

---

### 1️⃣ Active Reconnaissance

In **Active Reconnaissance**, the attacker **directly interacts** with the target system.

| Task                   | Tools                                            | Risk Level     |
|------------------------|--------------------------------------------------|----------------|
| Port Scanning          | nmap, Masscan, Unicornscan                       | High           |
| Vulnerability Scanning | OpenVAS, Nikto, Nessus                            | High           |
| Network Mapping        | Traceroute, Nmap                                 | Medium         |
| Banner Grabbing        | Netcat, curl                                     | Low            |
| OS Fingerprinting      | Nmap, Xprobe2                                    | Low            |
| Service Enumeration    | Nmap                                             | Low            |
| Web Spidering          | Burp Suite Spider, OWASP ZAP Spider, etc.        | Low–Medium     |

---

### 2️⃣ Passive Reconnaissance

In **Passive Reconnaissance**, the attacker gathers information **without direct interaction** with the target.

| Task                  | Tools                             | Risk Level  |
|-----------------------|-----------------------------------|-------------|
| Search Engine Queries | Google, DuckDuckGo, etc.          | Very Low    |
| WHOIS Lookups         | whois (CLI)                       | Very Low    |
| DNS Enumeration       | dig, nslookup, host, dnsenum, etc | Very Low    |
| Web Archive Analysis  | Wayback Machine                   | Very Low    |
| Social Media Analysis | LinkedIn, Twitter, Facebook, etc. | Very Low    |
| Code Repositories     | GitHub, GitLab                    | Very Low    |

---

## 📌 Notes
- Active reconnaissance carries higher risk as it can trigger IDS/IPS alerts.
- Passive reconnaissance is stealthier but provides less detailed system information.
- Combining both methods provides a more complete understanding of the target.

---

## 📚 References
- [OWASP – Information Gathering](https://owasp.org/www-community/Information_Gathering)
- [Nmap Official Guide](https://nmap.org/book/)
- [Recon-ng](https://github.com/lanmaster53/recon-ng)

---
**Author:** Pratik Das  
**Category:** Offensive Security / Web Reconnaissance
