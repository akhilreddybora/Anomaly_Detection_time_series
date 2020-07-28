# Anomaly_Detection_time_series

The program is used to identify any anomalies occuring in the time series data of S&P 500 Index using Keras API and LSTM autoencoder.

The data uploaded is already precprocessed for missing values.

The data is then split into train and test data for scaling operations using standard scaler.

Train and Test data are used to create time sequences to match the input shape of the LSTM network.

LSTM autoencoder network is created using Keras API.

Dropout layer was used as regularization and only a single layer of LSTM was used to keep the network simple.

The first two layers in the LSTM network acts as the encoder and last 3 act as the decoder for the network.

RepeatVector layer acts as the bridge between the encoder and decoder.

Model is then trained using Mean Absolute Error(MAE) as the loss function.

The model is then used to predict the anomalies in the test data.



