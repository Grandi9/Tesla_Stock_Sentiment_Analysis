# Tesla_Stock_Sentiment_Analysis

* Created a stock sentiment predictor based on the tweets on Tesla, and compared it to the Yahoo Finance data. Skills used: Spark, Big Data, Sentiment Analysis

* Used spark to clean and preprocess the tweets. 

* Textblob to process the sentiment analysis of the tweets

* Used ML models to predict the stock price change (Target variable: Trend - postive or negative based on the previous day).

* Based on the average value of the sentiment of tweets, the calculated value of trend (from sentiment analysis of tweets) is compared to the actual trend.

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


## Data Processing:


### Data Cleaning:

![image](https://user-images.githubusercontent.com/22790699/179430225-38f67b6e-e69b-4971-9d6b-c6fbab551c2a.png)

![image](https://user-images.githubusercontent.com/22790699/179430233-b32abd7b-35e9-4748-9845-4d1cb9b1d48a.png)


### Sentiment Analysis:

Used Text Blob Natural Language Processing (NLP) library to identify sentiment of the tweets.

![image](https://user-images.githubusercontent.com/22790699/179430262-c8b3364e-9e67-427b-9a17-68cac741dd63.png)

Grouping the sentiment by date:

![image](https://user-images.githubusercontent.com/22790699/179430288-2537550e-ea3c-4c1f-8a65-6d53d462001a.png)

* From the above plot, we can infer that the sentiments are normally distributed. Thus, i have taken the threshold as 0.16 to separate them into positive and negative sentiments.


![image](https://user-images.githubusercontent.com/22790699/179430482-d9f0ffae-380f-452d-bc42-532971357afc.png)


## Final Model

![image](https://user-images.githubusercontent.com/22790699/179430602-c2a1b36d-46d5-4ef6-9727-e375bd4857c3.png)

![image](https://user-images.githubusercontent.com/22790699/179430817-c04d6696-4507-4b9d-a878-5faa02c81563.png)


## Results:

### xgBoost
![image](https://user-images.githubusercontent.com/22790699/179430854-db0f2626-53e2-4f1d-8b42-86c9da31766e.png)

### Random Forest
![image](https://user-images.githubusercontent.com/22790699/179430877-8fbf5502-48de-45cf-a3a6-406d6bff153d.png)


