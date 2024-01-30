# Stocks-movement-prediction-ongoing
The notebook preprocesses with a list of stock symbols, using which it downloads the trading data of the stocks from Yahoo Finance, then performs technical calculations and tries to add features that will describe the sentiment attributed to the stock, among other things by calculating displacement ratios between the sectors and leading indicators \to the stock itself

The Lstm Feature_selection notebook is used to select features by using the lasso-type loss adding feature and thus adds the "absolute value of magnitude" of the coefficient as a penalty term to the loss function.
From that I will get the features selection I will work with later,  I handled tasks such as handling missing values, scaling features, creating sequences, addressing class imbalance and finding feature importance.

Coming up - LSTM prediction using the previous work
