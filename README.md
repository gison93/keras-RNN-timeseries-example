# Another example of how to build a multi-layer LSTM for time series prediction
Forked from [jaungiers/LSTM-Neural-Network-for-Time-Series-Prediction](https://github.com/jaungiers/LSTM-Neural-Network-for-Time-Series-Prediction)

## Data Source
This script assumes you have a relational database you can pull info out of to model. It uses sqlalchemy to connect. You must write the sql query yourself to get the time series out of the database correctly.

## LSTM model
You can alter the number of layers and [units](https://keras.io/layers/recurrent/#lstm) in the neural net by modifying the build_model method.

## Parameters
- sqlalchemy_conn_string: the connection string [formatted](http://docs.sqlalchemy.org/en/latest/core/engines.html) for sqlalchemy
- load_data.query: the sql query you execute to get the timeseries data
- epochs: number of epochs to train the model
- seq_len: number of time series points to use as input for the model
- prediction_length: number of time series points to predict into the future
- prediction_offset: Time in between predictions


