# LSTM Stock Predictor

![deep-learning.jpg](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Images/deep-learning.jpg?raw=true)

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the [Crypto Fear and Greed Index (FNG)](https://alternative.me/crypto/fear-and-greed-index/) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. You have been asked to help build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.

Action:

1. [Prepare the data for training and testing](#prepare-the-data-for-training-and-testing)
2. [Build and train custom LSTM RNNs](#build-and-train-custom-lstm-rnns)
3. [Evaluate the performance of each model](#evaluate-the-performance-of-each-model)

- - -

### Files

[Closing Prices Final Notebook](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Python%20Notebooks%20and%20CSV%20files/lstm_stock_predictor_closing.ipynb)

[FNG Final Notebook](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Python%20Notebooks%20and%20CSV%20files/lstm_stock_predictor_fng.ipynb)

### Prepare the data for training and testing

Use the FNG values to predict the closing price. For the closing price model, use previous closing prices to try and predict the next closing price.

Each model will use 70% of the data for training and 30% of the data for testing.

### Build and train custom LSTM RNNs

Use the same parameters and training steps for each model. This is necessary to compare each model accurately.

### Evaluate the performance of each model

> Which model has a lower loss?  
> The closing price predictor model had a lower loss than the FNG pridictor model.
> * FNG  
> 
> ![deep-learning.jpg](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Images/fngloss.JPG)
> * Closing Price Predictor  
> 
> ![deep-learning.jpg](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Images/sploss.JPG)
> 
> Which model tracks the actual values better over time?  
> The closing price predictor model tracks the actual values better over time.
> * Closing Price Predictor  
>![deep-learning.jpg](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Images/sptrack.JPG)
> * FNG 
>![deep-learning.jpg](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Images/fngtrack.JPG)
> Which window size works best for the model?  
> A window of 5 days in the closing price predictor model had the lowest loss:
>![deep-learning.jpg](https://github.com/DanEspin0821/deep_learning_14/blob/main/Final%20Files/Images/bslosscompare.JPG)
- - -

### Resources

[Keras Sequential Model Guide](https://keras.io/getting-started/sequential-model-guide/)

[Illustrated Guide to LSTMs](https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21)

[Stanford's RNN Cheatsheet](https://stanford.edu/~shervine/teaching/cs-230/cheatsheet-recurrent-neural-networks)


