# Stocks-movement-prediction-ongoing
The notebook preprocesses with a list of stock symbols, using which it downloads the trading data of the stocks from Yahoo Finance, then performs technical calculations and tries to add features that will describe the sentiment attributed to the stock, among other things by calculating displacement ratios between the sectors and leading indicators \to the stock itself

The Lstm Feature_selection notebook is used to select features by using the lasso-type loss adding feature and thus adds the "absolute value of magnitude" of the coefficient as a penalty term to the loss function.
From that I will get the features selection I will work with later,  I handled tasks such as handling missing values, scaling features, creating sequences, addressing class imbalance and finding feature importance.

Experiments-
1. In the first attempt at the direct approach, I will use the XGBoost algorithm in order to make a prediction using only today's features, that is, I will not give the model sequences from the previous few days. I will use this approach in order to get a basic algorithm to which I will compare my future attempts, with this approach I do not give a user of the data as a time series.
Also, I will examine the three types of labeling I created - daily, weekly and monthly

results- The results of the model are not good, but we will notice that the longer the prediction range is, the model gives less good performances

2. In this notebook I used a similar to the notebook in which I selected features, an LSTM algorithm that only on a sequence of the last X days (depending on the type of label) also, similar to the previous notebooks, I resampled the data to create a balance between the labeling and scaling of the data itself. You can see after each run the results of the models in different indices

results- The results of the model are not good, but we will notice that the longer the prediction range is, the model gives less good performances
