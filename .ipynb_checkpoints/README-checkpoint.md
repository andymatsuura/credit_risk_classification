# credit_risk_classification
module 20

In this challenge, various machine learning techniques are used to analyze a dataset of lending activity from a peer-to-peer lending company. This data is used to build a model to identify creditworthiness of borrowers

## Analysis

Factors for determining loan status considered in the dataset were:
*loan size
*interest rate
*borrowing rate
*debt to income
*number of accounts
*derogatory marks
*total debt

There were 77536 points in the dataset. First, the loan status (label) was separated from the rest of the data (features) and put into X and y variables. Then, the data was split into training and testing datasets. A logistic regression model was created, and fit with the training data. This model was then used to make predictions with the testing data. 

## Model Results

*Accuracy: 99%. In the classification report, the accuracy of the f1 score for the model is nearly perfect. 
*Precision: 94%. In predicting low-risk loans, the model is 100% precise. In predicting high-risk loans, the model is 89% precise. 
*Recall: 93%. The models recall was 100% in predicting low-risk loans, but correctly predicted high risk loans 87% of the time.
*It can be noted that the sample size of the low-risk loans was much larger than that of the high-risk loans (18746 vs 638)
## Summary

The model was perfectly accurate in predicting low-risk loans, which were a majority of the values in the dataset. Almost 90% precision and recall for the high-risk loans is not bad either, as some people were either mis-classified as low risk when they were high risk, or high risk when they were really low risk. These misclassifications represent a very small proportion of the total dataset. 

There were some inaccuracies when predicting high-risk loans, but with 99% accuracy across the training data set this model is recommended for use by the company, especially when it comes to low-risk lending.