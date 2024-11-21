# Spam Classifier Project
Overview
This project builds a Spam Classifier using the Apache SpamAssassin Public Corpus.
The goal is to classify emails as spam or ham (non-spam) based on their content. 
This involves:

- Preprocessing email data
- Feature extraction using word counts and vocabulary transformation
- Building and training a machine learning model for classification
- Evaluating the model for performance and reliability
-The classifier achieves high accuracy using a Logistic Regression model with
a feature engineering pipeline.

## Dataset
The dataset is sourced from the Apache SpamAssassin Public Corpus:

- Ham emails: Legitimate, non-spam emails (2,500 samples)
- Spam emails: Junk emails categorized as spam (500 samples)
  
Data Structure
Each email is stored in plaintext format and includes:

- Headers: Metadata like sender, subject, etc.
- Body: The actual email content.

## Steps in the Project

### Fetching the Data
Emails are downloaded from the Apache SpamAssassin repository and extracted into 
a local directory structure:

- easy_ham: Contains non-spam emails.
- spam: Contains spam emails.

### Parsing Emails
The Python email module is used to parse the email content into structured data, 
separating headers and the body text.

### Feature Engineering
Emails are transformed into numerical features through a pipeline:

- Word Count Extraction: Counting word occurrences in emails.
- Vocabulary Transformation: Limiting the vocabulary size to the most common words.
- Sparse Matrix Representation: Efficient representation of features using scipy.sparse.

### Model Training
The pipeline feeds the transformed features into a Logistic Regression model for classification:

- The pipeline automates preprocessing and feature extraction.
- Cross-validation ensures robustness of the model.

### Evaluation
The model is evaluated on the training set using cross-validation, achieving an average accuracy of 98.58%.
