# web-scraping
I used web scraping tools to collect data about the diplomatic activities of the country China.
Using the URL https://www.fmprc.gov.cn/mfa_eng, I scraped all the diplomatic activity news that that country has shared on their website. 
I excecuted it in 4 ways
1. Collecting links to all individual news pages
   The URL has a list of news about their diplomatic activities is available.
   Each item in the list has a link that leads to another web page, where more
   details are provided. I collected all of these links from all pages and save
   them in a .txt file. The script is download_links.py.
2. Downloading the HTML pages of the collected links
     I downloaded the HTML content of the links that I collected.
     Downloaded web page HTMLs and then parsing them locally.
     The script is save_html_pages.py
3. Parsing the downloaded HTML files and extracting the required information
     I read the downloaded HTML files, extracted the required information from them,
     and save them in a JSON file. From each HTML page,I extracted the date that the
     diplomatic activity occurred, the title of the news article, and the text content of the news article.
     The script is parse_html.py
5. Analyzing the scraped data
     I did some analyses that served as a sanity check for the
    quality of the collected data to make sure that the scraping was done correctly.
    The script is DataAnalysis.ipynb
