# Decision Tree Classifier
## Overview
The decision tree classifier model was implemented using Python(without any external libraries ML model) based on ID3 (Information Gain), C4.5(Gain Ratio), and CART(Gini Index) algorithms. The implemented model is trained and tested on the UCI Credit Approval dataset. The model can be used to reproduce the results mentioned in the results section with the same dataset. However, to train and test the model on different datasets, minor changes in the code preprocessing would be required.

## Pre-requisites

Python packages:

- Install the above packages using pip
    
    1. sklearn (Used to get kfold split and calculate performance metrics)
    2. Pandas
    3. NumPy
    4. math
    5. random

Files:
- Please ensure to place below the credit approval train and test data files as .data files and featuremapping.csv files in the Data folder
    - [training.data](Data/training.data)
    - [test.data](Data/test.data)
    - [featuremapping.csv](Data/featuremapping.csv)

## Steps to Follow
Follow the below steps to reproduce the results
1. Download the required packages listed in the Pre-requisites section
2. Place the [training.data](Data/training.data),  [test.data](Data/test.data) and [featuremapping.csv](Data/featuremapping.csv)files in Data folder inside the project directory(Directory where [DecisionTree.ipynb](Notebook/DecisionTree.ipynb) file is placed)
3. Update the [featuremapping.csv](Data/featuremapping.csv) to align with the column name and column type of input data
4. Open the notebook and run all the cells


## Final Performance Results
Below are the final performance results based on predictions made on [test.data](Data/test.data)
| Criterion | F1 Score | Accuracy |
| --- | --- | --- |
| ID3 | 0.81 | 0.821 |
| C4.5 | 0.80  | 0.821 |
| CART | 0.78 | 0.81 |
