# A Yen for the Future

The financial departments of large companies often have to make foreign currency transactions when doing international business, while hedge funds are also interested in anything that will provide an edge in predicting currency movements. Hence, both are always eager to gain a better understanding of the future direction and risk of various currencies. This project is about gaining a better understanding of prediction in the future movements in the value of the Canadian dollar versus the Japanese yen using Time Series forecasing and linear regression modelling.

## Methods and Techniques Used:

### For the time series forecasing

Firstly I have plotted the Settle price to check for long or short-term patterns.
Then I have decomposed the settle price into trend and noise using a Hodrick-Prescott filter
Then I went on to forecast returns using an ARMA model.
Followed by forecasing the exchange rate price using an ARIMA model.
Finally I've used GARCH to forecast the volatility in the near term.

### For the Linear Regression Forecasting

I have built a Scikit-Learn linear regression model to predict CAD/JPY returns with lagged CAD/JPY futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

Firstly, I had to create returns and lagged returns, and split the data into training and testing data as a part of Data preparation
Then I fit a linear regression model.
After which I made predictions using the testing data.
Lastly I evaluated the model using "out-of-sample" data (X_test and y_test) and in-sample data (X_train and y_train)

## Goal Of This Project: 

The main purpose of this project is to evaluate if one should buy a certain currency at a given time, to figure out whether the risks associated with the currency are expected to increase or decrease, to determine whether a time series and a linear regression model is appropriate to be used in real life and to evaluate the performance of a model comparing its performance in "out-of-sample" and "in-sample" data.

