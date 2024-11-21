# Titanic Classification Project
Overview
This project tackles the classic Titanic dataset, aiming to predict whether a passenger survived the Titanic disaster. 
Using machine learning techniques, we analyze and model the data to build a classification system that predicts 
survival based on attributes such as age, sex, class, and embarkation location.

## Objective
The goal is to create a predictive model that determines if a passenger survived based on their features. This involves:

- Data preprocessing (handling missing values, feature engineering, etc.)
- Exploratory Data Analysis (EDA)
- Model training and evaluation
- Optimization and testing on unseen data
- 
## Dataset
The dataset includes information about Titanic passengers:

- Train Dataset: Used for training the model.
- Test Dataset: Used to evaluate model performance.

Each dataset includes attributes like:

- PassengerId: Unique identifier
- Survived: Target variable (0 = did not survive, 1 = survived)
- Pclass: Ticket class (1st, 2nd, 3rd)
- Name: Passenger name
- Sex: Gender
- Age: Age in years
- SibSp: Number of siblings/spouses aboard
- Parch: Number of parents/children aboard
- Ticket: Ticket number
- Fare: Ticket fare
- Cabin: Cabin number
- Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Steps in the Project
### Data Fetching and Loading:

The data is downloaded programmatically from the GitHub repository and loaded into Pandas DataFrames for manipulation.
Data Preprocessing:

- Handling missing values (imputing missing Age and Embarked values).
- Encoding categorical variables (converting Sex to numerical values).

### Exploratory Data Analysis (EDA):

- Understanding data distributions.
- Investigating correlations and patterns.
- Visualizing survival rates across different groups (e.g., Pclass, Sex, Age).
  
### Model Building:

- Building a machine learning pipeline with preprocessing and training steps.
- Trying out multiple algorithms (Random Forest, SVM.).

### Evaluation:

- Measuring performance
- Cross-validation to ensure robustness.

## Requirements
Python 3.x
numpy
pandas
matplotlib
scikit-learn
