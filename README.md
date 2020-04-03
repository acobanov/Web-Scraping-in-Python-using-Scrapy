# Web-Scraping-in-Python-using-Scrapy

Writing custom scrapy spiders for large scale web scraping

  Scrapy is a Python framework for large scale web scraping. 
  It gives you all the tools you need to:
    -efficiently extract data from websites 
    -process them as you want
    -store them in your preferred structure and format

Let's start with web scraping by using my favourite tool called Anaconda.
Anaconda distribution is the world's most popular Python data science platform.


1.Install Scrapy package
(base) C:\Users\Ante>conda activate %your enivironment here%
(your environment) C:\Users\Ante>pip install scrapy


2. Create project's folder

Type the text below in Anaconda Prompt command line:

(base) C:\Users\Ante>conda activate %your enivironment here% 
(your environment) C:\Users\Ante>cd %desired location of your new scrapy project folder here%
C:\Users\Ante\...>scrapy startproject %project's name here% 

I have found these 3 things important when starting with Scrapy:

Comment 1:
Spiders are user-defined classes that Scrapy uses to scrape information from a website.
Custom Scrapy spiders must subclass scrapy.Spider class.

Comment 2:
Instead of implementing a start-requests() method that generates scrapy.Request objects from URLs,
you can just define a start_urls class attribute with a list of URLs. The list will then be used by
the default implementation of start_requests() to create the initial requaests for the spider.

comment 3:
parse() is Scrapy's deafault callback method, that is called for requests without an explicitly
assigned callback.

3. Extract the data

In order to extract desired data you will need to inspect HTML web page source code.
In order to find the proper CSS selectors to use, it is useful to open the response
page from the shell using view(response) or you can use browser's developer tools to 
inspect the HTML and come up with a selector.

I have found this link useful:
https://www.w3schools.com/cssref/css_selectors.asp






