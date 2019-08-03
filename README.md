
# Udacity project

# A closer look into the data of Seattle’s Airbnb market


Table of Contents:

1. The Libraries 

2. My Project Motivation

3. File Descriptions

4. Summary Of The Results

5. Acknowledgements


### The Libraries

The project was implemented using Anaconda distribution of Python 3.0. Moreover I have used the following python libraries:

1. Collections
2. Matplotlib
3. NLTK
4. NumPy
5. Pandas
6. Seaborn
7. Sklearn

### My Project Motivation

I was interested in exploring the AirBnB dataset for Seattle. I wanted to better understand the pricing trends, review sentiments and pricing prediction. Some of the questions that I have analyzed are:

How does the pricing increase or decrease by season?
What is the peak season in Seattle?
How does the pricing increase or decrease by neighborhood?
Which ones are the priciest neighborhoods in Seattle?
How does property types within neighborhoods impact price for the most expensive neighborhoods and most common property types?
How can we categorize reviews based on sentiments?
Can we map positive and negative sentiments from reviews to neighborhoods to understand which neighborhoonds rank higher on the positive sentiment scale and which ones rank higher on the negative sentiment scale?
Can we explore some of the worst reviews for additional insights?
Can we predict a price for a given listing?
What factors of the listing correlate best for predicting the price?
File Descriptions
The Jupyter notebook showcases the analysis done in order to explore the dataset, the data prepartion and wrangling as well as the building of prediction models in order to answer the questions above. The notebook contains markdown cells to help with documentation of the steps as well as to communicate findings based on each analysis.

For reference an HTML version of the notebook is also available.

Lastly, the seattle folder contains the dataset from Kaggle (https://www.kaggle.com/airbnb/seattle). It contains 3 files:

calendar.csv: calendar availability of listings and price
listings.csv: information about all the available listings
reviews.csv: listing reviews by the users
Summary Of The Results
The following key findings from the analysis are summarized below:

It was found that the peak season in Seattle is during the summer months from June to August, with the absolute peak being in July.
The "Southeast Magnolia" neighborhood was the priciest neighborhood in Seattle, followed by Portage Bay. Rainier Beach was the cheapest.
Looking further at neighborhoods and property types, I found out that houses in Portage Bay are the most expensive followed by houses in West Queen Anne and Westlake.
With the help of SentimentIntensityAnalyzer, I was able to map the reviews to their respective sentiments of positive, negative or neutral. I found out that 97.2% of reviews were mostly positive, with 1% negative reviews and 1.8% of reviews that were neutral.
By exploring review sentiments by neighborhoods, I found out that Roxhill, Cedar Park and Pinehurst were the neighborhoods with the most positive reviews, while University District, Holly Park and View Ridge ranked lower.
By exploring the worst reviews, I found out that SentimentIntensityAnalyzer associate non-English reviews with negative sentiments.
Using LinearRegression, I was able to predict price based on a prepped and cleaned dataset, with an r2score of 0.62 on both training and test datasets.
It was found that the features that had the most impact on price were a combination of host details as well as descriptive information about the listing.
