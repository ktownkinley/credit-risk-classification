# credit-risk-classification

## Overview of the Analysis

The analysis performed in this machine learning model was intended to create a way to predict whether a loan was in good standing or whether it was a high-risk loan based on the loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks and total debt. To accomplish this, I first split the known labels (good or bad loan) from the rest of the data and then split the data into a set of training data and testing data. The model was then created using a Logistic Regression and was fit with the training data. To evaluate the performance of the model, the model was then given the test data and predicted the outcome of the test data. It was then compared to the known outcomes of the test data to give a final score on accuracy, precision and recall.

## Results

* Machine Learning Model:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    * The accuracy of the model was 0.99 which is very high
    * The precision of a good loan was 1.00 which means the model is very good at predicting a good loan, but the bad loan had a precision of 0.84 which is concerning but the data for bad loans is very small which could introduce bias
    * The recall of a good loan was similarly 0.99, and the bad loan of 0.94 was a bit better than the precision 
    * The macro avg was 0.94 which does give a pretty good confidence that the model is performing decently

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Based on the results of the model, I would recommend using the model. After running the same model on a random sampling of equal weight (0s and 1s) in the dataset, it seemed to correct for the bias. However, the most important thing the model should be able to predict is the high-risk loans as those are the loans that are most likely to have adverse effect on the institution and is the main thing that we are trying to predict. If the model was run a couple more times with different random sampling and still gave a score > 0.9, I would recommend using the model