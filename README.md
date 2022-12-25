# Convolve-Hacakthon-2022
Classify software generated computer logs as either an anomaly or normal log based on the log text using ML/AI techniques. Currently using an LSTM network for classification and have qualified for the 2nd round.

The python notebook undersample_test.ipynb contains the prprocessing, implementation and resultant data.


# Approach

An undersampled dataset was created to train on due to the large class imbalance between anomalies and normal logs.
This was done by creating a dataset that contained every single abnormal log and an equal number of logs which were normal such that aprroximately all of its unique classed retained.

An LSTM model was then built to train the model for classification, which gave better results than GRUs or SimpleRNNs.
Due to the simple structure of the model, no dropout layer was implemented as it hurts the overall performance. 
