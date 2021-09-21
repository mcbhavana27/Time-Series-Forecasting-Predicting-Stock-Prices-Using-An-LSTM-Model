# Time-Series-Forecasting-Predicting-Stock-Prices-Using-An-LSTM-Model


** Data Preparation

I created a new data frame containing only the target variable - Closing stock price and converted it into an array to train the model. For this project, traning dataset had 80% of values. With time-series data, the sequence of values is important. 
<!-- The LSTM network expects the input data to be provided in 3D array structure: [samples, time steps, features]. Currently, the data is in the form: [samples, features] I transformed the train and test input data into the expected structure using numpy.reshape(). The first dimension is the number of records or rows in the dataset. The second dimension is the number of time steps. Since I used only one feature, i.e Close, the number of indicators will be one. -->

** Building the model and making Predictions

A Long Short-Term Model was built using Keras which had 30 units, 4 hidden layers and a dense layer (output) to predict the normalized closing stock price. The model was compile using the mean squared error as loss function and to reduce the loss or to optimize the algorithm, I used the Adam optimizer. Lastly, the model was fit and passed to the training features and a test data set was created to get predictions.

Result

![image](https://user-images.githubusercontent.com/58338319/134142657-06fc8e2e-14da-42b4-a5a6-a1fa6d557505.png)
