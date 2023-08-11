### Background
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
### Instructions
##### Split the Data into Training and Testing Sets
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.
##### Create a Logistic Regression Model with the Original Data
Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?
##### Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. 

# Credit Risk Analysis Report
## Overview - the purpose of this analysis
We are trying to see if a loan status to a borrower in the testing set would be a low or high risk. The way we do it is by splitting the dataset to training and testing sets that we have imported. The first part we handle is the training set in which helps build an Logistic Regression Model(`LRM`; Machine Learning Model) using sklearn(scikit-learn). Then we use this `LRM` to apply to the testing dataset to determine the risk. Once we get our results and learn about the certain biases it has, we use the RandomOverSampler to reshape the datasets.Once we have the reshaped dataset we have a new `LRM` that has a more accurate `LRM` than the first. 

## Results
* Machine Learning Model 1:
   * Accuracy: 99% (0.99)
   * Precision:
     * Healthy Loan - 100% (1.00)
     * High-Risk Loan - 87% (0.87)
   * Recall:
     * Healthy Loan - 100% (1.00)
     * High-Risk Loan - 89% (0.89)
* Machine Learning Model 2:
   * * Accuracy: 100% (1.00)
   * Precision:
     * Healthy Loan - 100% (1.00)
     * High-Risk Loan - 87% (0.87)
   * Recall:
     * Healthy Loan - 100% (1.00)
     * High-Risk Loan - 100% (1.00)

## Summary
The best `LRM` to use in my opinion would be the Machine Learning Model 2 due to the fact that it will predict less inaccurate results compared to Machine Learning Model 1. Even though the Precision is the same on both, the Accuracy has only a very small difference it does have higher accuracy and higher Recall that in the end will have a better prediction(precision) when using it. Thus giving us more accurate results when predicting.
