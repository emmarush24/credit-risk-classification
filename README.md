# credit-risk-classification

The goal of this analysis is to create a model that will accurately predict whether a loan is healthy or high risked based on factors such as the size of the loan, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt of an individual.

To achieve this goal I first exmined the data using the value_counts function to determine the balance of the target value. Using this function I could see the data held significantly more "healthy loans" than "high risk loans". I then split the data into training and test data. I then created a logistic regression model and trained it with the training data I created. Using the fitted model, I predicted the outcomes for the X test data. I then compared the predictions to the actual outcome. To understand the quality of the model, I produced a confusion matrix and classification report.

Results:
Machine Learning Model 1:
-Balanced Accuracy Score: 0.944
Precision for healthy loans: 1.00
Recall for healthy loans: 1.00
Precision for risky loans: 0.87
Recall for risky loans: 0.87

Machine Learning Model 2:
-Balanced Accuracy Score: 0.996
Precision for healthy loans: 1.00
Recall for healthy loans: 1.00
Precision for risky loans: 0.87
Recall for risky loans: 1.00

Overall, both models were good at predicting loan outcome based on the factors included. The second model was slighlty improved over the first model due to reduced misclassification of "bad loans". The first model does have the benefit from a banker perspective of having fewer false "healthy loans", however, the bank is being more risk averse under this model and reduces potential profit from loans that are misclassified as unhealthy. 