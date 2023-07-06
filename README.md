# Module-11-Data-Collection-Challenge

Part 1:

I began by inspecting the Mars news site (using the inspect function), and then started the scraping process: creating a Beautiful Soup object and extracting the desired elements (article text). Now we can use the Beautiful Soup object to store the text elements into an empty list, and by using a for loop, we can append dictionaries of article titles and summaries to the empty list.

Part 2:

For the second part, we need to scrape a large table off the mars facts website and I did so using Beautiful Soup much the same as in Part 1. However, I ran into a snag here where I was unsure of how to scrape the entire contents of the table and have the results print properly. By searching the Beautiful Soup documentation and a general stack overflow search I found these pages: https://www.crummy.com/software/BeautifulSoup/bs4/doc/ and https://python.plainenglish.io/introduction-to-web-scraping-using-python-and-beautifulsoup-bea91486c1d7 that provided insight into the ele.text.strip line that I ended up using to properly scrape the table. Now we are able to create a pandas dataframe from the scraped table, as well as change the data types for each column, and begin analysis. By using pandas and matplotlib functions, we're able to chart the temperatures for each month on mars as well as the atmospheric pressure, and to calculate the number of days in a martian year compared to an earth year.