# Cryptocurrency-Price-Prediction-using-LSTM
This project aims to demonstrate how to use the yfinance library to obtain historical cryptocurrency data and use it to train an LSTM model to predict future closing prices. The Ethereum-USD (ETH-USD) pair is used as an example, but the same approach can be applied to other cryptocurrencies and financial assets.

## Data acquisition and preprocessing
The first step is to download the historical data for the Ethereum-USD pair using the yfinance library. We choose the date range we want to use and we keep only the closing prices.

Next, we use the MinMaxScaler from the sklearn library to scale the prices between 0 and 1. This is a common technique used in time series forecasting to ensure that the model is not sensitive to the scale of the input data.

## Model construction and training
We use the Keras library to construct a simple LSTM model with one hidden layer and one output layer. The model is trained on the training set with 1 epoch.

## Results and evaluation
The predictions are made on the last 100 days of the dataset, and the results are plotted using matplotlib.

Additionally, the prediction for each day is printed on the console.

## Conclusion
This project demonstrates how to use the yfinance library to obtain historical cryptocurrency data, preprocess the data, and use it to train an LSTM model for price prediction. The results show that the model is able to capture the general trend of the Ethereum-USD pair over the last 100 days. However, it is important to note that this is a simple example and the predictions should not be taken as a financial advice.
