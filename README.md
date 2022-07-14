# lstm_stock_predictor
Build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.

# Model Comparison
After creating the LSTM models based on the FNG (Bitcoin Fear and Greed Index) and the closing crypto prices, it is clear that predicting closing prices based on previous closing prices is a much more effective practice. The Loss of the closing prices model reached 0.007 while the FNG model remained above 0.4 after 100 epochs. It is likely that the closing prices model may suffer from overfitting as well.

# Window size Comparison
The tested window sizes include 10 days, predicing the 11th day, 5 days, predicing the 6th day, and 20 days, predicting the 21st day. In all cases, the 10 day window provided the lowest loss function.

# Prediction Based on Closing Prices
stocks.plot(title="Actual Vs. Predicted Gold Prices")

# Prediciton Based on FNG Index
stocks.plot(title="Actual Vs. Predicted Gold Prices")