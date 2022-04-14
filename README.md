# Peer-To-Peer Lending Firm - Linear Regression Models

## Overview of the Analysis

The purpose of this application is to use the linear regression model to fit, model and predict outcomes on a set of data that contains data from thousands of loan data that includes the loan size, interest rate, borrower income, debt-to-income ratio, total_debt etc which is included in the lending_data.csv file which has been read into a DataFrame for analysis. . In addition, this application uses the RandomOverSampler module to re-sample the csv data to predict and compare the accuracy of the re-trained model using different sample/variables from the data.

Using the value_counts function on the targets, (2) labels amd numbers are generated. In this case, "0" is healthy loans and "1" is unhealthy loans. Balanced_accuracy_score generates an overall decimal value of accuracy while classification_report_imbalanced generates a dataframe which shows variables such as the accuracy, precision, recall and F1 score of the model.

The main model this application uses is the linear regression model that generates a line that trends with the overall data and uses that to predict which loans are healthy or unhealthy and compares the outcome of the model with the data set. Re-Sampling and re-training the model randomly and over samples the existing data and re-tests the model again in which theoretically the accuracy and precision of the resampled data with higher accuracy.

Live application link: https://github.com/davidlp94/12_DLP_Supervised_Learning/blob/main/credit_risk_resampling.ipynb

---

## Results

* Machine Learning Model 1 - Liner Regression:
    This linear regression model has a precision of 100% for healthy loans (18759 total) and a precision of 87% for unhealthy loans (625 total). The balanced accuracy loan value is 94.42%


* Machine Learning Model 2 - Logistic Regression Model with Resampling Data:
    This linear regression model has a precision of 99.99% for healthy loans (56277 total) and a precision of 99.99% for unhealthy loans (56277 total). The balanced accuracy loan value is 99.41%

---

## Summary

In conclusion, the Linear Regression model with Resampling of data has the highest accuracy, precision and balanced accuracy loan value out of the two regression models because it has a higher balanced accuracy loan value, precision and accuracy values (99.99%). These models play a very important role in determining healthy and unhealthy loans for a peer-to-peer lending firm to evaluate one's current risk in thier portfolio. Using this model, you can determine the amount of unhealthy loans currently active and compare them to the amount of healthy loans. It is important to predict the amount of unhealthy loans to determines one's current risk. Peer-to-Peer lending firms perform well when their ratio of healthy to unhealthy loans is higher!
