## Credit Risk Classifcation

## Overview of the Analysis 
The purpose of this analysis is to use a Logistic Regression model of supervised machine learning to predict the classification of loans into healthy or high-risk loan status categories. The data set includes 7 features: 
- Loan Size(Amount)
- Interest Rate
- Borrower Income
- Debt to Income
- Number of Accounts
- Derogatory Marks
- Total Debt
- Loan Status (Healthy or High-Risk)

After loading the dataset, the "loan_status" column was seperated from the rest of the DataFrame for the y variable, while all other columns were used for the X variable as the features.
The x and y variables were then split into train and test groups, which allows us to train the model with most of the data, and then compare predictions against the test set. 
The Logistic Regression model was then created and fit with the training data sets, and then predictions were made using the trained model. The accuracy of the model was analyzed using both a confusion matrix and a classification report. 

## Results 
* Logistic Regresression Learning Model:
    * Accuracy: 0.99
    * Precision: 1.0 with healthy loans, 0.85 with high-risk loans
    * Recall: 0.99 with health loans, 0.91 with high-risk loans
    * Confusion Matrix: 18663 true negative, 102 false positive, 56 false negative, 563 true positive

## Summary 
Overall this model performs well with an accuracy of 0.99. By looking at the precision and recall numbers, we can see the model more correctly predicts healthy loans than high-risk loans. Upon looking further into the high-risk loan predictions in the confusion matrix, 
we can see that the model predicts almost double the false positives (102) than the false negatives (56). I would recommend this model in this usage, as the bank will be looking to minimize any risk in their loans to customers and being more cautious with more 
false positives benefits the bank, while minimizing cases of false negatives which could cause more risk than predicted for the bank.  
