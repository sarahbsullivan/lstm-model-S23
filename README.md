# lstm-model-S23
## README.md
### Sarah Sullivan
### Created: October 6, 2023

This repository contains work I produced for the Spring 2023 Course at Johns Hopkins University: Gateway Data Science.

I train my model using historical price data of Apple stock (AAPL). It then predicts APPL prices for the first two weeks of 2023. Data is sourced from: 
https://www.nasdaq.com/market-activity/stocks/aapl/historical 
https://finance.yahoo.com/lookup

My code begins with exploratory data analysis of AAPL historical price data, including visualizations. 

I then train the data, using the TimeSeriesSplit method to avoid training based on future predictions. I include discussions of different weights for training vs. testing data.

I then create and initialize the model. Because this is time series data, I opt for a Recurrent Neural Network (RNN), choosing a Long Short-Term Memory (LSTM) Model. Discussions of my various choices are included. After evaluation, I choose Mean Squared Error as my loss function. 

Before making future predictions, I plot LSTM predictions against true values for historical data, showing the efficacy of my model. 

Finally, I apply the LSTM model to predict stock prices in 2023 and plot actual vs. predicted values. 

