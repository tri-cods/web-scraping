# Other Tools for Scraping Data

If out-of-the-box tools for web scraping do not meet your needs, you may need to write some code to collect your data. The Python programming language has some very helpful libraries that make web scraping possible.

These Python libraries may be of some use: 
- [Requests](https://docs.python-requests.org/en/master/index.html) allows you to do exactly what it says... request a web page from a URL. Crucially, requests returns the full HTML of a page in a usable form.
- [BeautifulSoup](https://pypi.org/project/beautifulsoup4/) is built to parse the HTML that you've got. If you've requested a page from the web you can isolate and collect data from specific locations in the DOM in the same way that you can with the browser extensions. You can also follow links to make additional requests and then parse those HTML responses.
- [Selenium](https://selenium-python.readthedocs.io/) and ChromeDriver together allow you to automate other browser behaviors. If, for example, you want to scrape 500 or more search results, but the search URL only displays the first 15 results and then requires you to scroll down to load more, the browser extensions and libraries listed above will not do the trick. These two libraries allow you to perform repetitive mouse and keyboard actions, populate and submit forms, even login to services behind an authentication layer (careful!).
- [Scrapy](https://docs.scrapy.org/en/latest/index.html) is a powerful Python library built for web scraping but also has a steep learning curve. 

With all of these options, you have a bit more control over what your results look like, and you can perform operations on your data (splitting full names into first name and last name fields, for example) before saving it as a file.

[<<<Back](04-scraper.md)
