Implemented a sentiment analysis tool that scrapes through major financial news sites to gather real-time financial news articles. Utilizing HTTP requests, BeautifulSoup4, and the Finnhub API (built on REST API), the script parses through relevant news articles of any U.S. ticker the user inputs and stores them into a dataframe with the help of Pandas and Numpy. To improve sentiment score accuracy, the script handles additional language processing techniques apart from the model itself. All news headlines are individually preprocessed to allow the model to interpret sentiment quicker and more efficiently. Perfoming lemmatization (most with the help of the NLTK library), removing stopwords, removing all unnecessary special characters, and making words lowercase are all ways that makes the model work smoother. Apart from preprocessing the data, the scrip also implements efficient sentiment scoring using additional language processing tehcniques to break down text into chunks, making the model more accurate. The tool has a built-in "grading system" that takes the aggregate mean of all sentiment scores on each individual headline to make a conclusion on general sentiment ranged from 1 to 5 - 1 being extremely bearish while 5 is extremely bullish. Finally, the script uses Matplotlib to help visualize sentiment using a histogram. This makes it accessible for the user to see the distribution of real-time sentiment through multiple sources.
