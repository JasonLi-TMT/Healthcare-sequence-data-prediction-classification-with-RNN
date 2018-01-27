# Healthcare sequence data prediction Classification with deep learning

## Data description:

In this project, I deal with healthcare sequence data, the data size is 60,000 * 476 matrix and it contains two part: clean data, dirty data,they both has size 30,000 * 476. Dirty data are continuous segment drawn randomly from clean data. 


The detail of data description could be found in the doc folder, there is a readme file there.

## Environment: 

1: Python environment setting is in the doc folder called environment.

2: Google Cloud: Including linux environment and GPU (Telsa K80). EC2 Url: https://35.227.55.209:5000 currently stopped due to cost, plz contact zl2528@columbia.edu to get access.

## Target:

1: Classify the data into ten labels.

2: Predict the next 25 sequence data with dirty data.

## Model:

1: Classification: GRU, LSTM, SimpleRNN, the model I trained is in the code-model folder saved as keras model. For GRU and Simple RNN, it achieve 93%, 91% accuracy rate, and for LSTM, it gets 83% accuracy rate

2: Predictions: GRU, LSTM, I classify the data into quantiles and use accuracy rate as target, but the result is not quite good, only 63% accuracy rate achieved due to time, compuational power & knowledge limitaion.

## some screenshot

![Screenshot](https://github.com/ZishuoLi/Healthcare_sequence_data_prediction-Classification_with_deep_learning/blob/master/image/GPU1.png)


![Screenshot](https://github.com/ZishuoLi/Healthcare_sequence_data_prediction-Classification_with_deep_learning/blob/master/image/GPU2.png)


![Screenshot](https://github.com/ZishuoLi/Healthcare_sequence_data_prediction-Classification_with_deep_learning/blob/master/image/GPU3.png)


![Screenshot](https://github.com/ZishuoLi/Healthcare_sequence_data_prediction-Classification_with_deep_learning/blob/master/image/GPU4.png)


![Screenshot](https://github.com/ZishuoLi/Healthcare_sequence_data_prediction-Classification_with_deep_learning/blob/master/image/GPU5.png)


![Screenshot](https://github.com/ZishuoLi/Healthcare_sequence_data_prediction-Classification_with_deep_learning/blob/master/image/GPU6.png)


![Screenshot](https://github.com/ZishuoLi/Healthcare_sequence_data_prediction-Classification_with_deep_learning/blob/master/image/GPU7.png)
