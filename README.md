# Ebay-webscraping-and-analysis
Web-scraped detailed product information from a 1000 product listings on eBay using Python
1. Save URLs of product listings into a folder with file name as item-id.html 
2. Loop through the downloaded pages, opens and parses them to a Python BeautifulSoup object. Then identify and select: seller name, seller score, item price, item price, list price, # items sold, title, returns allowed (true / false), shipping price, condition (e.g., used, new, like new, seller refurbished, ...)
3. Save information above into a SQL database - while saving, get rid of null values and convert prices from cents to dollars.(e.g., convert $12.34 into 1234 and $12 into 1200)
4. Run summary stats on each item: Summarize the differences in product sales when list_price is present and for different product conditions
5. Conclusion: 
Items which have a list price, generally have a higher seller score, higher number of items sold, higher number of items with returns allowed.
Based on the differences visible in the table and the box plots, the presence of list price seems to have a positive impact on total sales. Also, items with a list price and condition as new with tags were the most sold items on Ebay.
