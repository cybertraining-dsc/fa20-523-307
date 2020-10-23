# Analysis of Financial Markets based on President Trump's Tweets
Alex Baker, fa20-523-307, [Edit](https://github.com/cybertraining-dsc/fa20-523-307/blob/master/project/project.md)

{{% pageinfo %}}

## Abstract
Financial markets can be unpredictable as is but this unpredictability is increased by one man's Twitter account, President Trump. My goal is to use Twitter and finance datasets to see how these tweets affect the market.

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** analysis, finance, stock markets, politics


## 1. Introduction
For the final project, my focus will be on financial market reactions through the President's tweets. The plan is to utilize President Trump's tweets and stock market data to predict the market reaction based on what is going to be published. A feature that is being introduced is a way to craft tweets based on historical data to see how the markets will react if a tweet such as that is published. This can be useful to see how news from the president can cause an increase or decline in markets.

## 2. DataSets

The datasets that will be used are the tweets from President Trump's personal account as well as Yahoo fiance data. These will be gathered from their respected APIs. If needed, the following dataset from Kaggle (https://www.kaggle.com/austinreese/trump-tweets?select=trumptweets.csv) can be used in replace of Twitter's API for President Trump's tweets but are only available up to June 2020. Which leads to the objective for the project, based on the data collected, the program should be able to visualize and predict how the market will react when President Trump send out a tweet.

The data will span from President Trumps inauguration to the current day. To strengthen the prediction, even more, some code from the 2016 election’s analysis of markets may be utilized but the focus will be on the markets during the Trump administration. Rally data maybe introduced in order to have a deeper sense of some of the tweets when it comes to important news that is announces at President Trump's rallies. In order to have a realistic and strong prediction, the financial data needs to be aligned with the timing of tweets but news that has already started to affect the markets before a tweet has been sent out needs to be taken into account. 

## 3. Methodology/Process

The collection of finance and Twitter data will be used to visualize and predict the results. Some of Twitter or dataset data will need to be cleaned and classified to build the model. The methodology is composed of the following steps:

* Use data from President Trump's personal twitter to help visualize and create the model
* Use data from Yahoo finance API to help visualize and create the model
* Data cleaning and extraction.
* New data will be updated to keep up with the current time. 

## Data Cleaning and Aggregation

The first step is to clean the twitter and market data. Twitter's data is clean but in order to conduct the analysis needed, some of the columns need to be cleaned further. See the Data Cleaning section to see how this was accomplished. 

## Preliminary Analysis and EDA

Currently being conducted.

## Outline of plan

In the next seven weeks, these are the tasks that need to be accomplished.

* Week 9 - Week 10: Clean and preprocess the data needed for the project
* Week 10 - Week 11: Research what methods that should be used 
* Week 11 - Week 13: Preform sentiment analysis to find features and see if any correlation exists  
* Week 13 - Week 16: Build out NLP model 

## 4. Technologies used

Python, Jupyter notebook or collab, Pandas, Scikit-learn, Tensorflow/PyTorch

## 5. References

TBD