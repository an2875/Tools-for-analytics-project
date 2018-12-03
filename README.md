# __Tools-For-Analytics-Project__

## Sentiment analysis of tweets and its correlation with Stock prices

### Group name：You Guess 
### Section：002
#### _Team Members: Ashik Banger Veerappa, Dipanshu Gurwara, Xiyu Yang, Xinyi Cai_

## Goal & Motivation 

By utilizing sentiment analysis to predict stocks prices with respect to twitter feeds. We mainly focus on the technology industry as it’s highly correlated with market fluctuations and hence we pick up Google and Apple as two research objectives to implement our model. We used regression analysis to explore the relationships between tweets and stock prices. 

Regarding the stock prices, we used data visualization tools (plotly) to draw several graphs to present the price of the stock as time goes by. The sentiment analysis generated a dataframe with 9 columns: 8 emotions and the percentage change in stock prices, with date as index numbers. We also drew graphs to present each emotion sentiment with respect to percent change in stocks. 

## Data Sources:

We initially were planning to use tweepy package, but that does not provide the historical tweets and requires a twitter developer enterprise account. We went ahead with the historical tweets available of NASDAQ stocks like apple and google. We have used these two data files. We also obtained historical stock prices from yahoo finance using web scraping tools. 
For the stock market prices of the stocks, we have used the yahoo finance script and ran that on python for the required dates.

## Data Preprocessing:

We have uploaded the data into a pandas dataframe, cleaned the data, removed NaNs and took out the unwanted columns. We did this for AAPL,GOOG stocks for that time frame.

## Prediction:

We have used linear regression and random forest approaches to predict the stock prices for the following day. 
![Linear%20Regression.png](https://github.com/dipanshugurwara/Tools-for-analytics-project/blob/master/Linear%20Regression.png)

![Random%20Forest.png](https://github.com/dipanshugurwara/Tools-for-analytics-project/blob/master/Random%20Forest.png)

We have compared the two approaches for accuracy and prediction, and have gone with the approach that is more accurate.

## Results:

We achieved an accuracy of 67% with a percentage of stock correctly predicted as 85% with the linear regression algorithm. We were also able to achieve 61% accuracy and 64% percentage of stocks predicted correctly. Since the linear regression model approach was more accurate and identified a higher percentage of the stocks correctly, we have identified linear regression model as the final model to predict stocks using the sentiment of tweets.


