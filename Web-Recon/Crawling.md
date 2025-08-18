1. Crawling, often called `spidering`, is the `automated process of systematically browsing the World Wide Web

#### How web Crawler Work

Web Crawler are straightforward yet powerful.
	1. It start with the seed URL, which is the initial point to crawl.
	2. Crawler fetches this page, parser its content and extracts all its link.
	3. Then it adds the links to a queue and crawls them.

###### Types of Crawlers:

1. Breadth-First Crawling: Crawl prioritize depends on size.

2. Depth-First Crawling: Crawl prioritize depends on depth. 

##### Extracting Valuable Information

1. Links
2. Comments
3. Metadata
4. Sensitive Files

###### robot.txt

1. It is a simple text file that tells the web crawlers how to behave in the website or it contains certain set of rules for the web crawlers.

###### Understanding basic entries of robot.txt

* * wild card in the robot.txt file means the users.
* /<directory_name>

- Example:\
	- 
	`User-agent: *`
	`Disallow: /admin/`
	`Disallow: /private/`
	`Allow: /public/`
	`User-agent: Googlebot`
	`Crawl-delay: 10`
	`Sitemap: https://www.example.com/sitemap.xml`

1. all user agents are disallowed from accessing the /admin/ and /private/ directories
2. all users are allowed to access the /public/ directories
3. The `Googlebot` (Google's web crawler) is specifically instructed to wait 10 seconds between requests
4. The sitemap, located at `https://www.example.com/sitemap.xml`, is provided for easier crawling and indexing