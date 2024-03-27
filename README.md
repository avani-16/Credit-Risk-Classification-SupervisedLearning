# Credit-Risk-Classification

### Background
Used various techniques to train and evaluate a model based on loan risk. Used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

### Instructions
The instructions for this Challenge are divided into the following subsections:
  - Split the Data into Training and Testing Sets
  - Create a Logistic Regression Model with the Original Data
  - Write a Credit Risk Analysis Report

### Split the Data into Training and Testing Sets
1) Read the 'lending_data.csv' data from the 'Resources folder' into a Pandas DataFrame.
2) Create the labels set '(y)' from the “loan_status” column, and then create the features '(X)' DataFrame from the remaining columns.
   
   NOTE:
   A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

3) Split the data into training and testing datasets by using train_test_split.

### Create a Logistic Regression Model with the Original Data
Completed the following steps:
1) Fit a logistic regression model by using the training data (X_train and y_train).
2) Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
3) Evaluate the model’s performance by doing the following:
   - Generate a confusion matrix.
   - Print the classification report.


### Credit Analysis Report

   #### An overview of the Analysis:
   In this analysis, I have used various techniques to train and evaluate a model based on loan risk. Used a dataset of historical lending activity from a peer-to-peer 
   lending services company. First, splitted the data into training and testing sets and then created a Logistic Regression Model with the Original data. 
   Afterwards, evaluated the model's performance by generating Confusion Matrix and printed the Testing Classification Report.
   #### The results:
     - Accuracy score:
        The logistic regression model seems to predict high accuracy score of 0.99.
     - Precision score:
        The logistic regression model seems to predict the 0 (healthy loan) very well with precision score 1.00 
        but the 1 (high-risk loan) with 0.84.
     - Recall score:
        The logistic regression model seems to prdict the 0 (healthy loan) with 0.99 
        and 1 (high-risk loan) with 0.94.
   #### A summary:
      - From the confusion matrix, out of 18,765 'loan status' that are healthy (label 0), 
        the model predicted 18,655 as healthy correctly and 110 as incorrectly.
      - From the confusion matrix, out of 619 'loan status' that are high-risk (label 1), 
        the model predicted 583 as high-risk correctly and 36 as incorrectly.
      - This suggests that the model's ability to classify healthy loans is stronger than its performance with high-risk loans. 
      - Due to its accuracy, the machine learning model is highly recommended for both healthy and high-risk loans.
   
   



