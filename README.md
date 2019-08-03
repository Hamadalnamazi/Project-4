
# Udacity project

# A closer look into the data of Seattle’s Airbnb market


Table of Contents:

1. [The Libraries](https://github.com/Hamadalnamazi/Project-4/blob/master/README.md#the-libraries)

2. [My Project Motivation](https://github.com/Hamadalnamazi/Project-4/blob/master/README.md#the-My-Project-Motivation)

3. [File Descriptions](https://github.com/Hamadalnamazi/Project-4/blob/master/README.md#the-File-Descriptions)

4. [Summary Of The Results](https://github.com/Hamadalnamazi/Project-4/blob/master/README.md#Summary-Of-The-Results)

5. [Acknowledgements](https://github.com/Hamadalnamazi/Project-4/blob/master/README.md#Acknowledgements)


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

I was interested in exploring the AirBnB dataset for Seattle. I wanted to better understand the pricing trends and pricing prediction. Some of the questions that I have analyzed are:

Understand price increases/decreases by season and detect peak season in Seattle ?

what is the relation between neighborhoods , review and price how review and neighborhoods effect on price ?

Does accommodates make price higher and what is Top10 neighborhoods that accommodates effect in ?

### File Descriptions

The Jupyter notebook showcases the analysis done in order to explore the dataset, the data prepartion and wrangling as well as the building of prediction models in order to answer the questions above. The notebook contains markdown cells to help with documentation of the steps as well as to communicate findings based on each analysis.

For reference an HTML version of the notebook is also available.

Lastly, the seattle folder contains the dataset from Kaggle (https://www.kaggle.com/airbnb/seattle). It contains 3 files:

calendar.csv: calendar availability of listings and price
listings.csv: information about all the available listings
reviews.csv: listing reviews by the users

### Summary Of The Results


The following key findings from the analysis are summarized below:

It was found that the peak season in Seattle is during the summer months from June to August, with the absolute peak being in July.
The "Southeast Magnolia" neighborhood was the priciest neighborhood in Seattle, followed by Portage Bay. Rainier Beach was the cheapest.
Looking further at neighborhoods and property types, I found out that houses in Portage Bay are the most expensive followed by houses in West Queen Anne and Westlake.
With the help of SentimentIntensityAnalyzer, I was able to map the reviews to their respective sentiments of positive, negative or neutral. I found out that 97.2% of reviews were mostly positive, with 1% negative reviews and 1.8% of reviews that were neutral.
By exploring review sentiments by neighborhoods, I found out that Roxhill, Cedar Park and Pinehurst were the neighborhoods with the most positive reviews, while University District, Holly Park and View Ridge ranked lower.
By exploring the worst reviews, I found out that SentimentIntensityAnalyzer associate non-English reviews with negative sentiments.
Using LinearRegression, I was able to predict price based on a prepped and cleaned dataset, with an r2score of 0.62 on both training and test datasets.
It was found that the features that had the most impact on price were a combination of host details as well as descriptive information about the listing.
