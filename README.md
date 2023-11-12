This project was initiated as part of the GWU data bootcamp. It was part of a series of classes focused on web scraping and analyzing data produced by web scraping. 

The Python library we used for web scraping is Beautiful soup.

Instructions
Part 1: Scrape Titles and Preview Text from Mars News
Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.
1.	Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.
2.	Create a Beautiful Soup object and use it to extract text elements from the website.
3.	Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
1.	Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:
4.	Store all the dictionaries in a Python list.
5.	Print the list in your notebook.
6.	Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)

This part of the assignment was coded in the part_1_mars_news Jupiter notebook. In which we used Splinter and Beautiful Soup to scrape the website provided by the bootcamp. We then stored the output of the scraping in a list and closed the connection.

Part 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.
1.	Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.
2.	Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
3.	Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
1.	id: the identification number of a single transmission from the Curiosity rover
2.	terrestrial_date: the date on Earth
3.	sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
4.	ls: the solar longitude
5.	month: the Martian month
6.	min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
7.	pressure: The atmospheric pressure at Curiosity's location
4.	Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
5.	Analyze your dataset by using Pandas functions to answer the following questions:
1.	How many months exist on Mars?
2.	How many Martian (and not Earth) days worth of data exist in the scraped dataset?
3.	What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
1.	Find the average minimum daily temperature for all of the months.
2.	Plot the results as a bar chart.
4.	Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
1.	Find the average daily atmospheric pressure of all the months.
2.	Plot the results as a bar chart.
5.	About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
1.	Consider how many days elapse on Earth in the time that Mars circles the Sun once.
2.	Visually estimate the result by plotting the daily minimum temperature.
6.	Export the DataFrame to a CSV file.

In the part_2_mars_weather Jupiter notebook I scraped another website containing tabular data. I extracted the data and loaded it into a Pandas data frame. Then I ran several analysis on the data in the data frame. The graphs generated were also exported as a jpeg into the graph folder. I also exported the data to CSV and in JSON format.

Overall, a very interesting class. I have not used web scraping in my current work as most of the data we use is stored in SQL databases. This project was more a good to know vs a this is something I can implement on Monday kind of project.
