Creepy Crawlies are the tools that helps an attacker to automate the  crawling process making it faster and more efficient. 

### Popular web Crawlers:

1. Burp suite Spider
2. Owasp Zap
3. Scrapy
4. Apache Nutch

#### Scrapy:

1. installing Scrapy
	- `python3 -m venv ~/scrapy-env`
 
	- `source ~/scrapy-env/bin/activate`
	
	- `pip3 install scrapy`
	- 
	This is the framework installation
	
	- Tools:
		- ReconSpider:
		1. ` wget -O ReconSpider.zip https://academy.hackthebox.com/storage/modules/144/ReconSpider.v1.2.zip`
		2. `unzip ReconSpider.zip`
		3. `python3 ReconSpider.py <domain_name>`
		4. this will create `results.json` file.
###### Expected Results
{
    "emails": [
        "lily.floid@inlanefreight.com",
        "cvs@inlanefreight.com",
        ...
    ],
    "links": [
        "https://www.themeansar.com",
        "https://www.inlanefreight.com/index.php/offices/",
        ...
    ],
    "external_files": [
        "https://www.inlanefreight.com/wp-content/uploads/2020/09/goals.pdf",
        ...
    ],
    "js_files": [
        "https://www.inlanefreight.com/wp-includes/js/jquery/jquery-migrate.min.js?ver=3.3.2",
        ...
    ],
    "form_fields": [],
    "images": [
        "https://www.inlanefreight.com/wp-content/uploads/2021/03/AboutUs_01-1024x810.png",
        ...
    ],
    "videos": [],
    "audio": [],
    "comments": [
        "<!-- #masthead -->",
        ...
    ]
}



[[Crawling]]