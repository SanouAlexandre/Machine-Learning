# Deploy ML models with FastAPI, Docker, and Heroku
# Language Detection Project
This project aims to detect the language of a given text using machine learning techniques. The dataset contains text samples labeled with their respective languages.

## Project Structure

Loading the Dataset: Load the dataset into a pandas DataFrame.
Exploratory Data Analysis (EDA): Basic exploration to understand the distribution of languages in the dataset.
Text Preprocessing: Clean the text data by removing special characters and converting to lowercase.
Feature Extraction: Use Bag of Words model to convert text data into numerical features.
Train-Test Split: Split the data into training and testing sets.
Model Training: Train a Naive Bayes model on the training data.
Model Evaluation: Evaluate the model using accuracy, confusion matrix, and classification report.
Model Saving: Save the trained model and CountVectorizer for future use.

## Requirements
Python 3.x
pandas
numpy
scikit-learn
seaborn
matplotlib
pickle

## 1. Develop and save the model
app/model/La,guage_detection.ipynd
We use this code to develop and save the model

## 2. Create Docker container

```bash
docker build -t app-name .

docker run -p 80:80 app-name
```

## 3. Create Git repo

If you clone this repo this step is not needed. Or you can delete this git repo with `rm -rf .git` and start with a new one:

```bash
git init
git add .
git commit -m "initial commit"
git branch -M main
```

## 4. Create Heroku project to deploy our model

```bash
heroku login
heroku create your-app-name
heroku git:remote your-app-name
heroku stack:set container
git push heroku main
```
