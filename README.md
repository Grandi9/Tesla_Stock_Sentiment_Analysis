# Tesla_Stock_Sentiment_Analysis

* Created a stock sentiment predictor based on the tweets on Tesla, and compared it to the Yahoo Finance data.

* Used spark to clean and preprocess the tweets. 

* Textblob to process the sentiment analysis of the tweets

* Used ML models to predict the stock price change (postive or negative form the previous day) based on the avergae sentiment of the tweets during that day.

## Problem:

* Aim to predict the future stock price of TESLA based on historical stock price data and implement sentiment analysis of that data.

* Collected data from two different sources - Twitter and Yahoo finance. We did the sentimental analysis using the Kaggle dataset and used the previous stock price data from Yahoo finance to predict the future stock price.

* Data from Twitter - Sentiment has 16 features (1.1GB) (Used scrapped data from Tweepy bot from a Kaggle dataset)

* Data form Yahoo  - Previous stock price has 7 features (50 KB)


## Data Description:

### Twitter Data

![image](https://user-images.githubusercontent.com/22790699/179430148-f0a22810-9c2b-4ba2-a12e-da0cd4f6a882.png)

![image](https://user-images.githubusercontent.com/22790699/179430163-04bdfd9d-12f8-419e-b36d-68a09d62f13d.png)

### Yahoo Finance

![image](https://user-images.githubusercontent.com/22790699/179430173-7fce373e-7e69-41b4-8ac1-ac35e5fafd6b.png)

![image](https://user-images.githubusercontent.com/22790699/179430177-0338e4ee-f9ee-473d-84c2-b0de4e2de64a.png)

