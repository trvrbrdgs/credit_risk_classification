# Module 20 Report Template

## Overview of the Analysis

The purpose of the analysis was to determine whether or not the logisitcal regression model would accurately predict healthy loans and high-risk loans. 

The financial information was pulled from our lending_data.csv file. 

Variables included in this model included loan size, interest rate, borrower income, debt to income ratio, number of accounts, total debt, and derogatory marks. 

The stages of this machine learning process involved splitting the data into training and testing data. We used the test data to make predictions of our lending data and evaluated performance. By looking at the balanced accuracy score we found the test data to be 95% accurate. To verity this we created a confusion matrix and followed the matrix up with a classification report to further ensure accuracy. The results were favorable with 100% accuracy detection for healthy Lonas and about 85% accuracy on high-risk loans. 

We put the training data through the same process, but included a random over sampler function. The results were identical and will be listed below. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Model 1:
     precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384.



* Model 2:
     precision    recall  f1-score   support

           0       1.00      1.00      1.00     56271
           1       0.86      0.90      0.88      1881

    accuracy                           0.99     58152
   macro avg       0.93      0.95      0.94     58152
weighted avg       0.99      0.99      0.99     58152

## Summary

I would recommend this regression when predicting healthy loans. The ability to test for healthy loans was 100% according to both models. The ability to test for high-risk loans seems a bit low from an outsiders point of view. Not knowing the industry average of a model's ability to detect high-risk loans, this seems low. You may catch most of the high-risk loans, but it only takes one or two bad loans to ruin your fiscal year. Confidence for detecting high-risk loans is low. If another model were available that could put your high-risk loan detection above 90% that would be favorable. 
