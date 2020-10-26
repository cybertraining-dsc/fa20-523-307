# Analysis of Financial Markets based on President Trump's Tweets
Alex Baker, fa20-523-307, [Edit](https://github.com/cybertraining-dsc/fa20-523-307/blob/master/project/project.md)

{{% pageinfo %}}

## Abstract
In behavioral economics, it is said that emotions have an effect on individual's behavior and their chocie in their decision making process. This can be true for a society at large but can this apply to the leader of the free world? Here we will investigate the collective mood of President Trump's tweets are correlated to the value of the Nasdaq Stock Market (NASDAQ). The applications of sentiment analysis and machine learning methods will help find the correlation that we are looking for. President Trump's tweets will be used to predict the mood and the NASDAQ movements.   

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** analysis, finance, stock markets prediction, twitter, politics


## 1. Introduction
Financial markets have been an area of research in both academia and business. Predictions of the market has been growing in its accuracy with an every increasing amount of data used to test these models. "The Efficient Market Hypothesis (EMH) states that stock market prices are largely driven by *new* information and follow a random walk pattern"[1]. This shows that prices will follow news rather than previous and present prices. Information is unpredictable in terms of its release/publication showing market prices will follow a random walk pattern and the prediction can not be high. 

There are some problems that arrise with EMH. One problem is that "stock prices does not follow a random walk pattern and can be predicted to a certain degree"[2]. Another problem associated with EMH is with the information's unpreidctability, the unpredictability is called into question with the introduction of social media (Facebook, Twitter, blogs). The rise of social media can be a early indicator for news before it is released/published.    

## 2. DataSets

The datasets that will be used are the tweets from President Trump's personal account as well as Yahoo Fiance data. Financial data will be gathered from Yahoo Finance's API. President Trump's twitter data will be from the following dataset available on Kaggle (https://www.kaggle.com/austinreese/trump-tweets?select=trumptweets.csv).

The data will span from President Trumps inauguration to January 2020. To strengthen the prediction, even more, some code from the 2016 election’s analysis of markets may be utilized but the focus will be on the markets during the Trump administration. Rally data maybe introduced in order to have a deeper sense of some of the tweets when it comes to important news that is announces at President Trump's rallies. In order to have a realistic and strong prediction, the financial data needs to be aligned with the timing of tweets but news that has already started to affect the markets before a tweet has been sent out needs to be taken into account. 

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

[1] Goel, A. and Mittal, A., 2011. Stock Prediction Using Twitter Sentiment Analysis. [online] cs229.stanford.edu. Available at: <http://cs229.stanford.edu/proj2011/GoelMittal-StockMarketPredictionUsingTwitterSentimentAnalysis.pdf>.

[2] J. Bollen, H. Mao, and X. Zeng, “Twitter mood predicts the stock market,” Journal of Computational Science, vol. 2, no. 1, pp. 1–8, 2011. 