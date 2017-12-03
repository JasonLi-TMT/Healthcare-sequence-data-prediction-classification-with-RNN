# Data Science Assignment

The assignment can be found in **data_science_assignment.ipynb**. 

A detailed description of the datasets used for this assignment can be found [here](https://github.com/droicelabs/interview-assignments/blob/master/docs/DATASET.md).

## Part 1

In this part of the assignment, you will be performing analysis on a clean dataset **_D<sub>clean</sub>_**. 
This dataset consists of 30,000 data points in a fixed-length time series format, where each data point is assigned a label. 

**TODO:**
1. Analyze the dataset (open-ended). This can include statistics, visualizations, dimensionality reduction, or any other method you think is appropriate. Document in the README your process, why you chose to analyze the data the way you did, and any interesting findings. 
2. Train a classifier on the dataset and report the results. Include information about the methods you used and the results in the README.

This part of the assignment is designed to show us your general approach to data science/machine learning, as well as provide some information about your comfort with standard analysis techniques. 

## Part 2

In this part of the assignment, you will be performing analysis on a corrupted dataset **_D<sub>corrupt</sub>_**. 
This dataset is drawn from the same source as **_D<sub>clean</sub>_** but does not contain duplicate data points. 
This dataset consists of 30,000 data points in a variable-length time series format, where each sample *x<sub>i</sub>* has been randomly extracted from a fixed-length sequence.
Additionally, each data point has a label, which is unknown. 

**TODO:**
1. Classify each data point. With your submission, include the results as a shape = (30000,) Numpy array named **corrupt_labels.npz** with labels in [0,1,...,8,9]. 
2. Find the optimal alignment of each data point. With your submission, return the results as a shape = (30000,2) Numpy array named **corrupt_alignments.npz** with the beginning and ending index for each data point.
3. Document the methods/strategies you used in parts 2.1 and 2.2 in your README.

This part of the assignment will be graded on both a) the correctness of the results from parts 2.1 and 2.2, and b) the creativity and general approach used to tackle this problem. 
