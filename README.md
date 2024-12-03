# Google-Stock-Prediction
## DSCI575 Final Project - Comparing Traditional ARIMA Models to a SimpleRNN and LSTM Model for Google Stock Price Data
### Claire Kintzley

## Problem Statement
Accurately modeling and forecasting stock price data is often challenging due to high volatility and complex market trends. Traditional time series models, like ARIMA, have been widely used in forecasting because of their interpretability and straightforward assumptions about data patterns. However, advancements in deep learning, specifically Long Short-Term Memory (LSTM) networks, present an opportunity to capture more complex trends that may improve prediction accuracy. This project seeks to address the question: _How does the predictive performance of a traditional ARIMA model compare to that of an RNN and LSTM model when forecasting the daily opening prices of Alphabet (Google) stock?_ 

## Project Overview
This project involves developing and comparing three different models for predicting Alphabet Inc.'s (GOOG) daily opening stock prices. The models used for forecasting include:

- **ARIMA (AutoRegressive Integrated Moving Average)**: A traditional statistical model that is suitable for forecasting univariate time series data by capturing patterns of past observations.
- **RNN (Recurrent Neural Network)**: A neural network model designed for sequence prediction, making it capable of learning from previous time steps in the data.
- **LSTM (Long Short-Term Memory)**: An advanced type of RNN that addresses the vanishing gradient problem and can capture long-term dependencies in sequential data.

The project focuses on comparing the performance of these models using key metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE). The next-day prediction (first day of training data) will also be compared.

## File Summaries

### StockPredictionARIMA.ipynb
This notebook implements the ARIMA model for forecasting the daily opening stock prices of Alphabet Inc. (GOOG). It includes data preprocessing, model fitting, and evaluation using performance metrics like MSE and MAE, with visualizations of the forecasted vs. actual stock prices.

### StockPredictionSimpleRNN.ipynb
In this notebook, an RNN model is built and trained on the Alphabet stock data to predict the daily opening prices. It covers data preprocessing, model construction, training, and evaluation, with visualizations comparing the model's predictions to the actual data.

### StockPredictionLSTM.ipynb
This notebook demonstrates how to use an LSTM model to predict Alphabet's daily opening stock prices. It involves preparing the data, building the LSTM model, training it on the stock data, and visualizing both training and testing predictions for performance evaluation.

## Findings
- The LSTM model provided the most accurate predictions, followed by the Simple RNN, and lastly the ARIMA model.
- While ARIMA is a useful model for simpler time series problems, the RNN and LSTM models showed a marked improvement in predicting more complex patterns in stock price data.
- The LSTM model demonstrated superior performance, confirming the effectiveness of deep learning models in forecasting financial data compared to traditional methods like ARIMA.


Data source: https://www.kaggle.com/datasets/henryshan/google-stock-price

Additional sources:
- https://www.geeksforgeeks.org/time-series-forecasting-using-recurrent-neural-networks-rnn-in-tensorflow/
- https://www.kaggle.com/code/ozkanozturk/stock-price-prediction-by-simple-rnn-and-lstm
- https://ieeexplore.ieee.org/abstract/document/8614252