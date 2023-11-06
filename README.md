# Classification using KNN on Vertebral Column Data Set

## Introduction
This repository contains an analysis of the Vertebral Column Data Set, a biomedical dataset that classifies patients into Normal (NO) and Abnormal (AB) categories. The binary classification task aims to distinguish between NO (0) and AB (1) using the K-Nearest Neighbors (KNN) algorithm. 

## Dataset
The Vertebral Column Data Set contains six biomechanical attributes derived from the pelvis and lumbar spine. You can download the dataset from the following link:
[Vertebral Column Data Set](https://archive.ics.uci.edu/ml/datasets/Vertebral+Column)

## Pre-Processing and Exploratory Data Analysis
### Scatterplots
Visualize the data by creating scatterplots of the independent variables, using color to distinguish between classes 0 and 1.

### Boxplots
Generate boxplots for each independent variable, using color to differentiate between classes 0 and 1.

### Train-Test Split
Split the data into a training set and a test set. Select the first 70 rows of Class 0 and the first 140 rows of Class 1 as the training set, with the remaining data as the test set.

## K-Nearest Neighbors (KNN) Classification
### KNN Implementation
Implement KNN using the Euclidean metric for distance calculation.

### Testing KNN
1. Test all data in the test database with various values of `k`. Take decisions by majority polling. Plot train and test errors for different `k` values in reverse order, e.g., from 208 to 1, with smaller increments if needed.

2. Determine the most suitable `k` (denoted as `k*`) based on train and test errors. Calculate the confusion matrix, true positive rate, true negative rate, precision, and F1-score when `k = k*`.

3. Optimize for the best test error rate by using a subset of the training set. Plot the best test error rate against the size of the training set (`N`), with `N` ranging from 10 to 210. For each `N`, select the optimal `k` from a set starting from `k = 1` and increasing by 5.

4. Create a "Learning Curve" to visualize the relationship between training set size and the best test error rate.

## Variants of KNN
1. You can explore different variants of the KNN algorithm to enhance classification performance.



