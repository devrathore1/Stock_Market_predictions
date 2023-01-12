# Stock_Market_predictions


# Project Title

The data that it is accompanied with is actual stock data with fictitious dates and tickers. 
To give me exogenous aspects to consider, I have have eliminated the previous day's closing price but kept other genuine stock data up to that point. 
Prices are all as of closing. Assume you can purchase at closing.
## Data
Real world stock market data
## Key Pointers

What data pre-processing techniques did I use?

Describe the method for choosing features.

Why did I select the models I did?

Give an overview of each model's performance before choosing one to use going forward.

The stock price forecast should be printed.
## Final Analysis

Data pre-processing:

New column was created for date and concatenated for further use to pandas array in one of the models instead of using Index. 
Data visualization was done to check if the data is skewed or have inconsistencies. 
Data was scaled, normalized & standardized. Jupyter notebook & screenshots are attached below.
As per the model’s requirements, in LSTM, MinMaxScaler was used for scaling.



Feature Selection:
Feature selection was primarily done for ARIMA model, attached below. However, for ARIMA model part 2, LSTM & Facebook Prophet model, only index & MMAX values were considered. 
For feature selection: SelectKBest from from sklearn .feature_selection was used.


Model Performance:

LSTM:
LSTM prediction: $115.413055
One form of recurrent neural network called Long Short-Term Memory (LSTM) is widely utilized to learn order dependency in situations involving sequence prediction. The LSTM is particularly effective at forecasting stock values because it can store historical data and learn patterns and trends from it to predict the future.  

ARIMA prediction:
An ARIMA model is a dynamic univariate forecasting method for predicting the future values of a time series. Because it is critical to identify a model to analyse stock price movements with adequate information for decision making, the ARIMA model for stock price prediction is recommended.

Facebook Prophet:  
Price prediction $96.7757
Prophet package is developed by Facebook for forecasting time series data based on an additive model incorporating annual, monthly, and daily seasonality, as well as holiday impacts. It works best with time series with substantial seasonal effects and data from several seasons.

## Goal(s)

Utilizing the graph of my choice, plot the daily returns of MMAX across the whole time.

