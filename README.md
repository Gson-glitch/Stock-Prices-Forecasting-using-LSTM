# Stock Prices Prediction Model using LSTM

## Overview
This project aims to develop a stock prices prediction model using LSTM (Long Short-Term Memory) neural networks. The model was trained on historical stock prices data to predict the future trends of the stock prices. 

## Dataset
The dataset used for this project is the historical stock prices data of Google, Microsoft, Facebook, Amazon, Tesla, and Apple, obtained from Yahoo Finance. The dataset consists of daily stock prices data spanning the last 10 years.

## Preprocessing
Before feeding the data to the LSTM model, some preprocessing steps were, including:
- Checking for and handling missing values
- Normalizing the data
- Splitting the data into training and testing sets

## LSTM Model Architecture
This is a two-layer LSTM model with one input layer, one hidden layer with 128 units, and one output layer. The input shape is defined as (x_train.shape[1], 1), where x_train is the training data, and the second parameter is the number of features.

The first LSTM layer has 128 units and returns sequences, which means that it produces an output for each input timestep. The second LSTM layer has 64 units and does not return sequences, which means that it produces an output for the last timestep only.

The output of the second LSTM layer is passed through a fully connected Dense layer with 25 units, followed by a final output layer with one unit, which produces the predicted stock price value.

The model will be trained on the preprocessed training data, and its performance will be evaluated on the preprocessed testing data.

## Evaluation Metrics
We will evaluate the performance of the LSTM model using the following metrics:
- Root Mean Squared Error (RMSE)


## Usage
To use the stock prices prediction model, follow these steps included in the Jupyter Notebook File, preferrably on [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb)


## Contributors
- Gloryson Ondanje

