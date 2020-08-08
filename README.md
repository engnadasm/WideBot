# WideBot_Task_1 : Getting to Philosophy
## the problem statement :
Please write a Python script to check the "Getting to Philosophy" law.
https://en.wikipedia.org/wiki/Wikipedia:Getting_to_Philosophy
Clicking on the first link in the main body of a Wikipedia article and repeating the process
for subsequent articles would usually lead to the article Philosophy.
The program should receive a Wikipedia link as an input, go to another normal link and
repeat this process until either Philosophy page is reached, or we are in an article without
any outgoing Wikilinks, or stuck in a loop.
A "normal link" is a link from the main page article, not in a box, is blue (red is for
non-existing articles), not in parentheses, not italic and not a footnote. You don't have to
check style tables or other fancy things, it is enough that the script works with the current
Wikipedia style (for example you can use 'class' attribute in Wikipedia tags). For easy
validation, please print all visited links to the standard output.
Use a 0.5 second timeout between queries to avoid heavy load on Wikipedia (sleep function
from time module).
## First,I install dependencies
like: BeautifulSoup, urllib, time, sys & requests where :

Beautiful Soup is a Python package for parsing HTML and XML documents (including having malformed markup, i.e. non-closed tags, so named after tag soup). It creates a parse tree for parsed pages that can be used to extract data from HTML.

Urllib module is the URL handling module for python. It is used to fetch URLs.

urllib.parse for parsing URLs

time to handle time-related tasks.

requests module allows you to send HTTP requests using Python.

## Second define two function where are called
  ### 1- find_first_link
    which take url of the first articl and get the first link in page by using dependencies and Build a full url &
    if the the current articl doesn't contains any links return.
    
   ### 2- continue_scraping
    which take all visited_urls and target_url and return true or false after a group of choices
