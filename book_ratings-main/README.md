# ﻿DSTI ML Project A22 Cohort (Group 16):
The aim of this project is to train and evaluate different models that predict a book’s rating from a GoodReads dataset.

## 0) Environment and Kernel set up
Before running the notebook, we will create a new kernel from a virtual environment that we will create for the project specifically.\
We will use:
- **python** to create a virtual envionment
- **pip** to install all necessary packages
- **ipython** to create a kernel from our virtual environment

|  |  |
| --- | --- |
| ```venv_path``` | **path-to-project\\.venv-book** |
| ```kernel_path``` | **%USERPROFILE%\\AppData\\Roaming\\jupyter\\kernels\\.venv-book** |  

Once the packages are installed, refresh the page and select the **.venv-book** kernel before the imports:
- `Kernel` > `Change kernel` > `.venv-book`

## 1) Data Exploration
- 1.1) Null Values & Data Types
- 1.2) Unique Identifiers
- 1.3) Numeric, Non-numeric & Categorical variables
- 1.4) Study of Non-numeric variables
- 1.5) Study of Numeric variables

## 2) Feature Engineering
- 2.1) Pre-processing of Dataset
- 2.2) Feature Analysis (Correlation Matrices)

## 3) Model & Feature Selection
- 3.1) Variation of Feature Sets
- 3.2) Data Split
- 3.3) Model Training & Evaluation
- 3.4) Feature Selection (Empirical)
- 3.5) Model Finetuning
- 3.6) Model Finetuning through GridSearch

## 4) Deployment
- 4.1) Preprocessing function
- 4.2) Loading Data From Cloud (DVC + Google drive)
- 4.3) Loading Model From Cloud (DVC + Google drive)
- 4.4) Making Predictions

## 5) Appendix: Hosting & Versioning
For the versioning and hosting of the code, data and models we combined:
- Github
- DVC (Data Version Control)
- Google drive : https://drive.google.com/drive/u/0/folders/1dR0CdRVGBb4tKxbVoCbqSfeWz7gpLtWv

Then, using the DVC API, we fetch the models and data from the cloud.

Ref: https://dvc.org/doc/use-cases/versioning-data-and-models

## Contributors
- Stuart Yoel TURNER
- Gaston AVELINE
- Alexandre SANOU
- Sy Lucien TRAORE
