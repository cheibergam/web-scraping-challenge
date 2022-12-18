# Mission to Mars :: web-scraping-challenge

The main objective of this project is to implement a full web-scraping and data analysis project for the Mission to Mars

The project is organised in two main deliveries:
* Deliverable 1: Scrape Titles and Preview Text from Mars News
* Deliverable 2: Scrape and Analyze Mars Weather Data

## Resources
* [Mars NASA news site](https://redplanetscience.com/)
* [Mars Temperature Data](https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html)
* [Mars Temperature Data Site](https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html)

## Delivery 1 :: Scrape Titles and Preview Text from Mars News

 1.  Use automated browsing to visit the  [Mars NASA news site](https://redplanetscience.com/). Inspect the page to identify which elements to scrape.

 2.  Create a Beautiful Soup object and use it to extract text elements from the website.

 3.  Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:Store each title-and-preview pair in a Python dictionary. And, give each dictionary two keys:  `title`  and  `preview`.
	 * Store all the dictionaries in a Python list.
	 * Print the list in your notebook.
 4.  Optionally, store the scraped data in a file or database (to ease sharing the data with others). To do so, export the scraped data to either a JSON file or a MongoDB database.


## Delivery 2

 1. Use automated browsing to visit the [Mars Temperature Data Site Links to an external site.](https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html). Inspect the page to identify which elements to scrape.

 2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas  `read_html`  function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
    
 3.  Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
	 * `id`: the identification number of a single transmission from the Curiosity rover
	 * `terrestrial_date`: the date on Earth
	 * `sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
	 * `ls`: the solar longitude
	 * `month`: the Martian month
	 * `min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
	 * `pressure`: The atmospheric pressure at Curiosity's location

 4.  Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate  `datetime`,  `int`, or  `float`  data types.

 5.  Analyze your dataset by using Pandas functions to answer the following questions:
	 1. How many months exist on Mars?
	 2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
	 3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
		 * Find the average the minimum daily temperature for all of the months.
		 * Plot the results as a bar chart.
	 4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
		 * Find the average the daily atmospheric pressure of all the months.
		 * Plot the results as a bar chart.
	 5.  About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
		 * Consider how many days elapse on Earth in the time that Mars circles the Sun once.
		 * Visually estimate the result by plotting the daily minimum temperature.

 6.  Export the DataFrame to a CSV file.

## Results and Analysis
The results and analysis are detailed in the files enclosed in this repository:
* **Delivery 1:** `part_1_mars_news.ipynb`
* **Delivery 2:** `part_2_mars_weather.ipynb`