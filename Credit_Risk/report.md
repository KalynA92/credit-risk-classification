## Overview of the Analysis

The purpose of this analysis was to build a machine learning model to predict healthy and high-risk loans to credit applicants. The financial information included in the data was; the size of the loan, interest rate, borrower's income, debt compared to income, number of accounts, derogatory marks, total debt, and the loan status either healthy or high-risk. I seperated the loan_status to act as the labels and the rest of the data as the features. I used value_counts to determine the number of loans for each type either healthy or high-risk. I split the data into training and testing datasets by using train_test_split. I fit a logistic regression model by using the training data (X_train and y_train). I evaluated the model’s performance by calculating the accuracy score of the model, generating a confusion matrix, and printing the classification report. The same methodolgy was used to predict a Logistic Regression Model with Resampled Training Data using the RandomOverSampler module from the imbalanced-learn library to resample the data.

## Results

* Machine Learning Model 1:
  * Accuracy - 0.94 (The model is predicting both healthy and high-risk loans at a very successful rate)
  * Precision - Safe: 1.00 and Risk: 0.87 (All safe loans predicted accurately while 87% of high-risk loans predicted accurately)
  * Recall - Safe: 1.00 and Risk 0.89 (All safe loans correctly identified while 89% of high-risk loans correctly identified)

* Machine Learning Model 2:
  * Accuracy - 0.99 (the model is predicting both healthy and high-risk loans at an almost perfect rate)
  * Precision - Safe: 1.00 and Risk: 0.99 (Both safe and high-risk loans predicted pretty much perfectly)
  * Recall - Safe: 0.99 and Risk: 0.99 (Both safe and high risk loans are correctly identified)

## Summary

It seems like machine learning model 2 would prove better results. Both models are able to predict the success of a loan candidate very well. Machine learning model 1 has an accuracy of 94% which is very promising. The healthy loans predicted and identified accurately as confirmed by the precision, recall, and f1 scores. The high-risk loans scores aren't as reliable but still do hold some merit. With precision, recall and f1 scores of 0.87, 0.89 and 0.88 respectively, the model is still proving to be effective but, it would be up to the loaner if they'd be willing to take the risk I assume based on the amount being loaned. Machine learning model 2 has the same results for the healthly loans but, the high-risk loans scores all increase to 0.99. This shows that with a little more data, it's possible to increase the predictability. The data is skewed abit more to the healthy loans overall, it would be better to have a more even split dataset to work with. 

