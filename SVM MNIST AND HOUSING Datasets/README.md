# 1. SVM Classifier on MNIST Dataset
## Overview
This project demonstrates the implementation of a Support Vector Machine (SVM) classifier 
on the MNIST dataset, a popular dataset of handwritten digits used for image classification 
and machine learning benchmarking. The classifier is trained using Scikit-Learn and includes
preprocessing, training with different SVM configurations, hyperparameter tuning, and evaluation.


## Dataset Preparation
The MNIST dataset is loaded using fetch_openml.
The dataset is split into a training set (60,000 samples) and a test set (10,000 samples).
The data is already shuffled, so additional shuffling is not required.

## Linear SVM Classifier
A linear SVM classifier (LinearSVC) is trained on the raw dataset.
Results:
Accuracy without scaling: 83.5%
After scaling the data with StandardScaler: 92.1%

## Non-Linear SVM with RBF Kernel
A non-linear SVM classifier (SVC with RBF kernel) is trained on a subset of the scaled dataset 
(10,000 samples).
Results:
Accuracy on the training set: 94.5%

## Hyperparameter Tuning
A randomized search with cross-validation is performed to tune hyperparameters C and gamma.
Search space:
gamma: Reciprocal distribution between 0.001 and 0.1
C: Uniform distribution between 1 and 10
Results:
Best parameters: C=7.12, gamma=0.00103
Cross-validated score: 86.4% (on 1,000 samples)

## Final Model Training
The best estimator is retrained on the full scaled training set.
Results:
Training set accuracy: 99.7%
Test set accuracy: 97.3%


# 2. SVM Regressor on California Housing Dataset

## Overview
This project demonstrates the implementation of a Support Vector Machine (SVM) regressor on 
the California Housing dataset. The goal is to predict median house values in California based 
on various features using Scikit-Learn. The project includes preprocessing, training with both 
linear and non-linear SVM regressors, hyperparameter tuning, and evaluation.

## Dataset Preparation
The California Housing dataset is loaded using fetch_california_housing().
The dataset is split into a training set (80% of the data) and a test set (20% of the data).

## Data Scaling
Feature scaling is performed using StandardScaler to improve the performance of SVM models.

## Linear SVM Regressor
A linear SVM regressor (LinearSVR) is trained on the scaled training set.
Results:
Training set Mean Squared Error (MSE): 0.964
Training set Root Mean Squared Error (RMSE): 0.982

## Non-Linear SVM Regressor with RBF Kernel
A non-linear SVM regressor (SVR with RBF kernel) is trained using hyperparameter tuning.
Hyperparameter tuning is performed using randomized search with cross-validation.
Search space:
gamma: Reciprocal distribution between 0.001 and 0.1
C: Uniform distribution between 1 and 10
Results:
Best parameters: C=4.75, gamma=0.0797
Training set RMSE: 0.573

## Evaluation on Test Set
The best model is evaluated on the test set.
Results:
Test set RMSE: 0.593


# Requirements
Python 3.7+
Scikit-Learn
NumPy
SciPy
