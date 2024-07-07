# Predicting Paper Breaks in Multivariate Time Series Data #
## Overview ##
This project aims to predict rare events, specifically paper breaks, in multivariate time series (MTS) data from a pulp-and-paper industry. The goal is twofold:

Predict the occurrence of a paper break before it happens.
Identify the variables that are likely to cause the paper break, enabling proactive measures to prevent it.

## Dataset ##
The dataset (Data.csv) consists of multivariate time series data collected from sensors in a pulp-and-paper industry. It includes various features (variables) recorded over time, with the target variable indicating the occurrence of a paper break.

## Approach ##
### Data Preprocessing: ###

* Read and preprocess the MTS data using pandas.
* Identify and handle missing values, if any.
* Standardize non-categorical data using StandardScaler.
* Perform PCA for dimensionality reduction to capture 95% variance.
### Modeling: ###

* Train an SVM classifier (SVC) to predict paper breaks based on preprocessed features.

### Evaluation: ###
* Evaluated model performance using metrics like F1 score, recall, and precision.
* Assess feature importance to identify variables contributing most to predicting paper breaks.

### Output: ###
* Provided predictions on test data.
* Display metrics and insights regarding the identified causal variables.
