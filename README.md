# scrapeEmailAddress
###Step 1: Import modules<br>
1.re for regular expression matching operations <br>
2.requests for sending HTTP requests<br>
3.urlsplit for breaking URLs down into component parts<br>
4.deque is a list-like container with fast appends and pops on either end<br>
5.BeautifulSoup for pulling data out of HTML files of websites<br>
6.pandas for formatting emails into a DataFrame for further manipulation<br>
<br>
###Step 2: Initialize variables
Then, we initialize a deque for saving unscraped URLs, a set for scraped URLs, and a set for saving emails scraped successfully from the website.
<br>
Elements in Set are unique. Duplicate elements are not allowed.
<br>

###Step 3: Start scraping
1.First, move a url from unscrapedto scraped.
<br>
2.Then we use urlsplit to extract different parts of the url.
<br>
urlsplit() returns a 5-tuple: (addressing scheme, network location, path, query, fragment identifier).
<br>Sample input & output for urlsplit()
<br>
3.Sending an HTTP GET request to the website.
<br>
4.Extract all email addresses from the response using a regular expression, and add them into the email set.
<br>5. Find all linked URLs in the website.

<br>

###Step 4: Export emails to a CSV file


