# Analysis of Financial Markets based on President Trump's Tweets
Alex Baker, fa20-523-307, [Edit](https://github.com/cybertraining-dsc/fa20-523-307/blob/master/project/project.md)

{{% pageinfo %}}

## Abstract
In behavioral economics, it is said that emotions have an effect on individual's behavior and their choice in their decision making process. This can be true for a society at large but can this apply to the leader of the free world? Here we will investigate the collective mood of President Trump's tweets are correlated to the value of the Nasdaq Stock Market (NASDAQ). The applications of sentiment analysis and machine learning methods will help find the correlation that we are looking for. President Trump's tweets will be used to predict the mood and the NASDAQ movements.   

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** analysis, finance, stock markets prediction, twitter, politics


## 1. Introduction
Financial markets have been an area of research in both academia and business. Predictions of the market has been growing in its accuracy with an every increasing amount of data used to test these models. "The Efficient Market Hypothesis (EMH) states that stock market prices are largely driven by *new* information and follow a random walk pattern"[1]. This shows that prices will follow news rather than previous and present prices. Information is unpredictable in terms of its release/publication showing market prices will follow a random walk pattern and the prediction can not be high. 

There are some problems that arise with EMH. One problem is that "stock prices does not follow a random walk pattern and can be predicted to a certain degree"[2]. Another problem associated with EMH is with the information's unpredictability, the unpredictability is called into question with the introduction of social media (Facebook, Twitter, blogs). The rise of social media can be a early indicator for news before it is released/published. This project is attempting to predict the market based on how the President tweets. This currently has not been done according to my research.   

## 2. DataSets
In this project, two datasets will be used - 
* The NASDAQ values from November 2016 to January 2020. This data was obtained through Yahoo! Finance and includes Date, Open, High, Low, Close, Adj Close, and Volume for a given day.

* President Trump's tweets during the periods of November 2016 to January 2020 is over 41,000 tweets. The data includes id, link, content, date, retweets, favorites, mentions, hashtags, and geo for every tweet in the time frame. Since the performance of the prediction is on a daily basis, tweets will be split up by Date. This data is available on Kaggle (https://www.kaggle.com/austinreese/trump-tweets?select=trumptweets.csv).


To strengthen the prediction, even more, some code from the 2016 election’s analysis of markets may be utilized but the focus will be on the markets during the Trump administration. Rally data maybe introduced in order to have a deeper sense of some of the tweets when it comes to important news that is announces at President Trump's rallies. In order to have a realistic and strong prediction, the financial data needs to be aligned with the timing of tweets but news that has already started to affect the markets before a tweet has been sent out needs to be taken into account.  

## Data Cleaning and Preprocessing

The data obtained needs to be cleaned and pre-processed in order to make it reliable for analysis.  

### Twitter Data

When importing the Twitter data, there are several things that are noticed when printing the first five rows. Three of the columns mention, hashtags, and geo are currently showing NaN. After calculating the missing values, all the values in these columns are missing or are zero so we can drop these columns from the dataframe.

The tweets are one of the last columns needed to be cleaned. The text of the tweets needs to be uniformed in order to conduct analysis. Removing punctuations was the first step followed by removing content specifically seen in tweets. These could be the word retweet, the hashtag symbol(#), the @ symbol followed by a username, and any hyperlinks that could be in a tweet. 

### Stock Data

Stock data has a unique set of challenges when it comes to cleaning. Unlike tweets, stock data is only available Monday through Friday and is not available for holidays that the market is closed. In order to have a complete dataset, several options are available. One option is to drop the tweets that fall on a weekend. This would not be useful since markets can react to news that happens on the weekend. Another option is to approximate the missing values in the stock data. This has not been conducted yet. 

## 3. Methodology/Process

The collection of finance and Twitter data will be used to visualize and predict the results. Some of Twitter or dataset data will need to be cleaned and classified to build the model. The methodology is composed of the following steps:

* Use data from President Trump's personal twitter to help visualize and create the model
* Use data from Yahoo finance API to help visualize and create the model
* Data cleaning and extraction.
* New data will be updated to keep up with the current time. 

## Preliminary Analysis and EDA

### Twitter Data

When starting to conduct preliminary analysis and exploratory data analysis (EDA), it is helpful to first check for any null values in the data and there are no null values in the twitter data. 

The date column is a column that is needed to track the amount of tweets per month and year. In the column, the timestamp and the date are combined so this need to be separated in several ways. The first being separating the date from the timestamp into its own column. This is followed up by separating the date into 4 columns for day, month, year and month-year in order to track tweets based on specified criteria. 

After graphing the amount of tweets per year, the observation is that 2016 and 2020 have a low tweet count. The reminder is that the data starts in November 2016 making 2016 have two months of data compared to 2020 with only one month being January. From 2017 through 2019, we can see that the amount of tweets increases by almost a thousand every year. The tweets per month tell a different story. The amount varies greatly over the years with the greatest amount being near the end of 2016 and the beginning of 2017.   

### Stock Data

Similar to the twitter data, checking for null values is important but since the data is from Yahoo! Finance there are no missing values on the days that the markets are opened. 

Once graphing the open and closed prices of the NASDAQ, there seems to be an general upwards trend in the market over the time period. 

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