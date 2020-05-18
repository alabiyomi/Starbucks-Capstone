# Udacity Data Scientist Nanodegree Capstone Project

This repository has all the code and report for my Udacity Data Scientist Nanodegree Capstone project.

## Starbucks Capstone Challenge: Using Starbucks app user data to predict effective offers

### 1. Installations
This project was written in Python, using Jupyter Notebook on Anaconda. The relevant Python packages for this project are as follows:

- pandas
- numpy
- math
- json
- sklearn.model_selection (train_test_split module)
- sklearn.preprocessing (StandardScaler, PolynomialFeatures)
- from sklearn.tree (DecisionTreeClassifier,DecisionTreeRegressor)
- sklearn.ensemble (RandomForestClassifier)
- sklearn.metrics (mean_squared_error,classification_report)
- sklearn.linear_model (Ridge)
- time
- sklearn.model_selection (GridSearchCV)
- matplotlib

### 2. Project Motivation

**Build a model that predicts whether a customer would respond to an offer or not.**

***The entire analysis would contain below steps:***

1. Analyse each of the portfolio, profile and transaction data.
2. Clean and tranform each of the portfolio, profile and transaction data.
3. Combine portfolio, profile and transaction data.
4. Select a performance metric to analyse performance of the model and to compare different models.
5. Compute the performance of a baseline model against which performance of other different models would be compared.
6. Select best performing model based on the metric and training time.
7. Calculate the feature importances given by best estimator of the trained model.
8. Compute the performance of best model on test set and visualize the performance via confusion matrix plot.


The resulting solution will be that best model would be able to determine which customers would respond.








### 3. File Descriptions
This repo contains 4 files. The report of my project is called 'Starbucks Capstone Challenge - Using Starbucks app user data to predict effective offers.ipynb'. 
The data used in the project is in the files portfolio.json, profile.json and transcript.json.


portfolio.json - 10 rows, 6 columns.
  id (string) - offer id
  offer_type (string) - type of offer ie BOGO, discount, informational
  difficulty (int) - minimum required spend to complete an offer
  reward (int) - reward given for completing an offer
  duration (int) - time for offer to be open, in days
  channels (list of strings)


profile.json - 17000 rows, 5 columns. e
  age (int) - age of the customer
  became_member_on (int) - date when customer created an app account
  gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
  id (str) - customer id
  income (float) - customer's income


transcript.json - 306534 rows, 4 columns. e
  event (str) - record description (ie transaction, offer received, offer viewed, etc.)
  person (str) - customer id
  time (int) - time in hours since start of test. The data begins at time t=0
  value - (dict of strings) - either an offer id or transaction amount depending on the record


