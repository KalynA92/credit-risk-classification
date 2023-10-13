# credit-risk-classification

## Task

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

1. Split the Data into Training and Testing Sets

2. Create a Logistic Regression Model with the Original Data

3. Write a Credit Risk Analysis Report

## Description

I started by importing the necessary modules. I read the csv file and created a Pandas DataFrame. I seperated the data into labels and features(loan_status being the label and the rest of the data the features). I checked the balance of the variables using value_counts. I imported the train_test_learn module and split the data using train_test_split. I imported the LogisticRegression module from SKLearn, instantiated the Logistic Regression model and fit the model using the training data. I made predicitions using the testing data. Evaluated the model's performance by calculating the accuracy score of the model, generating the confusion matrix and printing the classification report. I used the same methodolgy to predict a logisitc regression model with resampled training data using the RandomOverSampler module from imbalanced-learn library. I completed the credit risk analysis report found in the credit_risk folder of this repository named 'report.md'.

## References

RandomOverSampler module from imbalanced-learn library references:

https://machinelearningmastery.com/random-oversampling-and-undersampling-for-imbalanced-classification/ 

http://glemaitre.github.io/imbalanced-learn/generated/imblearn.over_sampling.RandomOverSampler.html

https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.RandomOverSampler.html
