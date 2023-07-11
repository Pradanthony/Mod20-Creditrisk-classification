Report on Credit risk classification

Overview of the Analysis
The analysis was performed on a lending data in csv format. The data contained details on loans and the borrowers and most importantly the loan status.
Using the data on loans (Size and Interest rate) and borrowers (Income, Debt to income, Accounts, Derogatory marks and Total debt) we must predict the loan status accuractly to help future decision making on loan approval.
The loan status variable is the outcome based on which the loan approval decision should be made so it is very important to predict this accuratelky with our model.
This means in our analysis the Y variable (outcome) is the loan status while the rest were X variables.
The train test split method was used to check the accuracy of the Y (loan status) prediction.
Linear Regression model was used to predict the Loan status (outcome) and the train test data used to check the accuracy of the prediction.
Since the data was imbalanced with more 0 loan status (healthy loan) than 1 loan status (high risk loan), the Random Oversampled method was used to balance the data.
The linear regression was tested with ROS data to check the accuracy of the outcome (loan status) with a balanced data set.

Results
