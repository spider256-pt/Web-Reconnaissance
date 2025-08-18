
Virtual Hosting can be defined as the way for web-server to differentiate between domains, sub-domains or even separate websites with distinct content.

## How virtual Hosts work ?

The ability of virtual Hosting is leveraged by the ==***Http Host***== header, a piece of information included in every HTTP request.

###### The key difference between Vhosts and Subdomain:

- Vhosts: A feature of the web-server that allows the host to access the main domain and the different sub-domain of the same domain for a particular host. 
	- Example:
		host: 10.129.x.x
		Hosted domains:
			inlanefreight.com
			dev.inlanefreight.com
			ns1dev.inlanefreight.com
			
- Subdomains: Are the extension of a main domain name. Subdomain typically have their own DNS records. They can be used to organise different sections or services of a website.
	- Example:
		blog.inlanefreight.com
		etc.

#### Types of Virtual Hosting:

1. Name-based Virtual Hosting
2. Ip-based Virtual Hosting
3. Port-based Virtual Hosting

## Virtual Host Discovery Tools

1. Gobuster- often use for directory/ virtual host discovering
	- `gobuster vhost -u <target_website> -w <wordlist> --append-domain`
	
		1. -u: flag specifies the target URL
		2. -w: flag specifies the wordlist
		3. --append-domain: flag appends the base domain to each word in the wordlist
		4. -t: flag increases the number of threads for faster scanning
		5. -k: flag can ignore SSL/TLS certificate errors
		6. -o: flag to save the output to a file for later analysis

2. Feroxbuster- same function but known for its speed

3. ffuf- used for pattern based brute forcing and also for v-host discovery.
	- `ffuf -u <target_url> -H "<host_server>" -w <wordlist> -fs <size>`  
	- use ffuf for vhosts enumeration and pattern based dir brute-forcing.

[[DNS{Domain Name System}]]
