Report on Credit risk classification

Overview of the Analysis
The analysis was performed on lending data in csv format. The data contained details on loans and the borrowers and most importantly the loan status.
Using the data on loans (Size and Interest rate) and borrowers (Income, Debt to income, Accounts, Derogatory marks and Total debt) we must predict the loan status accurately to help future decision making on loan approval.
The loan status variable is the outcome based on which the loan approval decision should be made so it is very important to predict this accurately with our model.
This means in our analysis the Y variable (outcome) is the loan status while the rest were X variables.
The train test split method was used to check the accuracy of the Y (loan status) prediction.
Logistic Regression model was used to predict the Loan status (outcome) and the train test data used to check the accuracy of the prediction.
Since the data was imbalanced with more 0 loan status (healthy loan) than 1 loan status (high risk loan), the Random Oversampled method was used to balance the data.
The linear regression was tested with ROS data to check the accuracy of the outcome (loan status) with a balanced data set.

Results
Model 1
•	Balanced Accuracy Score – 0.95
•	Precision – 1.00 for 0 (healthy loan status) and 0.86 for 1 (high risk loan status)
•	Recall - 1.00 for 0 (healthy loan status) and 0.91 for 1 (high risk loan status)
•	F1-score - 1.00 for 0 (healthy loan status) and 0.88 for 1 (high risk loan status)

Model 2 (ROS method)
•	Balanced Accuracy Score – 0.99
•	Precision – 1.00 for 0 (healthy loan status) and 0.85 for 1 (high risk loan status)
•	Recall - 0.99 for 0 (healthy loan status) and 0.99 for 1 (high risk loan status)
•	F1-score - 1.00 for 0 (healthy loan status) and 0.92 for 1 (high risk loan status)

Summary
In our environment of predicting the loan status, it is very important to predict the high-risk loans (outcome of 1). The main purpose of this prediction is to reduce the risk of high-risk loans in order to avoid loan default. 
The first model with logistic regression had a good balanced accuracy score of 0.95 but it was not good at predicting the high-risk loan status. The recall score of 0.91 confirms this and a wrong prediction of 9% with a high-risk loan status is not good. 
However, this data was imbalanced, so we need to try the second method of Random Oversampled (ROS) data to test the linear regression again with the resampled data.
The predicted results were much better with the ROS method. With the ROS method the balanced accuracy score increased to 0.99 and most importantly the Recall score of high-risk loan status (1) increased to 0.99. The risk is predicting the wrong outcome for high-risk loan status has been greatly reduced by using the ROS method.
Therefore, I would recommend the Random Oversampled with logistic Regression method to analyze and predict the outcome of the Loan status.
