# deep-learning

Deep learning recurrent neural networks are used to model bitcoin closing prices. One model (lstm_stock_predictor_fng) will use the FNG indicators to predict the closing price while the second model(lstm_stock_predictor_closing) will use a window of closing prices to predict the nth closing price. Each model uses 70% of the data for training and the remaining 30% of the data for testing. MinMaxScaler is used to fit and reshape feature data for the model.

## Tools used

numpy, pandas, hvplot, matplotlib, tensorflow, keras, from tensorflow: Sequential, LSTM, Dense, Dropout, from sklearn: MinMaxScaler

## Questions

1. The model using closing price had a much lower loss than the model using fng scores to predict closing prices at 0.03240999951958656 v 0.1087786927819252 in the fng model.
2. As seen in the plots below it is clear the the model using closing price to make predictions follows the actual vaules better over time.
3. The default window of 10, 5 appears to be the best window for the model. 
