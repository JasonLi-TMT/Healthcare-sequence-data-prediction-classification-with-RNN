# Deep Learning 

A detailed description of the datasets used for this assignment can be found at dataset folder

## Part 1

In this part of the assignment, you will demonstrate basic proficiency coding in deep learning libraries/Tensorflow. 
You will be training neural networks on a clean dataset **_D<sub>clean</sub>_**. 
This dataset consists of 30,000 data points in a fixed-length time series format, where each data point is assigned a label. 
A basic network has been provided in [Keras](https://keras.io/). 


1. Implement custom objective functions
   - Cross-entropy (done)
   - Cosine distance
   - General regression error
   - Hinge loss
2. Implement basic neural network architectures for time series classification
   - MLP (done)
   - RNN 
   - CNN (1D convolutions)

When implementing the custom objectives, use only basic Tensorflow operations (i.e., do not use the pre-defined loss functions in **tf.nn** or **tf.losses** libraries).

When implementing neural network architectures, use Keras or Tensorflow. Feel free to add any techniques/regularization you think will make your model better, and justify your choices in the README. This is a limited assignment, so you can also discuss methods that you would consider if you had more time. Bonus points are awarded for code that is flexible and generalizable with respect to architecture and hyperparameter search for ease of integration in machine learning pipelines. 

## Part 2

Implement a classification task on a corrupted dataset **_D<sub>corrupt</sub>_**. 
This dataset is drawn from the same source as **_D<sub>clean</sub>_** but does not contain duplicate data points. 
This dataset consists of 30,000 data points in a variable-length time series format, where each sample *x<sub>i</sub>* has been randomly extracted from a fixed-length sequence.
Additionally, each data point has a label, which is unknown. 


1. Classify each data point. Feel free to use any of the network architectures/objectives above, and to perform any analysis or pre-processing on the data that may improve the classification accuracy. With your submission, include the results as a shape = (30000,) Numpy array named **corrupt_labels.npz** with labels in [0,1,...,8,9]. 

## Part 3

1. Modify the objective function to predict the next 25 samples in the time series. 
2. Predict the next 25 samples for each data point in **_D<sub>corrupt</sub>_**. With your submission, include the results as a shape = (30000,25) 
