# Epileptic-Seizure-Recognition-Using-ANN
Recognition of Epileptic Seizures through attributes provided
## Dataset

### Source:
```
Qiuyi Wu 
School of Mathematical Sciences 
Rochester Institute of Technology 
email: qw9477'@'rit.edu 

Ernest Fokoue 
School of Mathematical Sciences 
Rochester Institute of Technology 
email: epfeqa'@'rit.edu 
Phone: 585 739 6893
```
### Attribute Information:

The original dataset consists of 5 different folders, each with 100 files, with each file representing a single subject/person. Each file is a recording of brain activity for 23.6 seconds. The corresponding time-series is sampled into 4097 data points. Each data point is the value of the EEG recording at a different point in time. 

The response variable is y in column 179 

y contains the category of the 178-dimensional input vector. Specifically y in {1, 2, 3, 4, 5} 

- 5- eyes open, means when they were recording the EEG signal of the brain the patient had their eyes open 
- 4- eyes closed, means when they were recording the EEG signal the patient had their eyes closed 
- 3- Yes they identify where the region of the tumor was in the brain and recording the EEG activity from the healthy brain area 
- 2- They recorder the EEG from the area where the tumor was located 

All subjects falling in classes 2, 3, 4, and 5 are subjects who did not have epileptic seizure 

- 1- Recording of seizure activity 

The Explanatory variables X1, X2, ..., X178 

Each 178-dimensional vector contained in a row, represents a randomly selected 1-second long sample picked from the single file. Recall that 
each file is a recording of brain activity for 23.6 seconds. The corresponding time-series is sampled into 4097 data points.


### Abstract: 
This dataset is a pre-processed and re-structured/reshaped version of a very commonly used dataset featuring epileptic seizure detection.
```
Data Set Characteristics:  Multivariate, Time-Series

Number of Instances: 11500

Area: Life

Attribute Characteristics: Integer, Real

Number of Attributes: 179

Associated Tasks: Classification, Clustering

Missing Values? N/A
```

## Artificial Neural Network

Code:

- Keras
- scikit-learn
- pandas
- matplotlib

Execution:

- Execution was done on spyder using python 3.5

Feature Scaling:

-Feature Scaling has been applied to the inputs using standard scaler

Layers:

- Input layer
- Hidden layer
- Output layer

### Classification Basis
> Although there are 5 classes,binary classification has been performed. 
> Namely class 1 (Epileptic seizure) against the rest, changed to 0.
