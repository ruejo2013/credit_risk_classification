# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:
The credit risk analysis is use to determine creditworthiness of borrowers, by a peer-to-peer lending service company.

Using historical finiacial data, which included customers loan amount (loan size), interest rate (interest_rate), income (borrower_income), DTI (debt_to_income) number of accounts (num_of_accounts)
payment default (derogatory_marks), total debt (total_debt) and loan status (loan_status) which marks the customers creditworthiness ie likelihood of the customer defaulting on a loan. 

The dataset use for training and testing the model had 77,536 rows and 8 columns, with 75,036 '0 healthy loan' and 2,500 '1 high-risk loan'.

To build, test and evaluate the model, these steps were followed:

1. Load the data
2. Prepare the data, separate the data into labels and features.
3. Split the data to training and testing set
4. Instantiate the model (using the original data set)
5. Fit the data to the model ie train the model
6. Predict the data (test the model)
7. Evaluate the model performance
8. Resample (oversample) the data, even the labels.
9. Create another instance of the model
10. Fit the new model with the over-sampled (label) data
11. Test the model 
12. Evaluate the model



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
 1. Balance accuracy score : 95% accurate
 2. Precision: The model was 100% precise in predicting '0 healthy loans' and 85% precise inpredicting '1 high-risk loans'
 3. Recall: The model was 99% correctly classified '0 healthy loans' and 91% correctly classified '1 high-risk loans'



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
 1. Balance accuracy score : 99% accurate
 2. Precision: The model was 100% precise in predicting '0 healthy loans' and 84% precise inpredicting '1 high-risk loans'
 3. Recall: The model was 99% correctly classified '0 healthy loans' and 99% correctly classified '1 high-risk loans'

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

The over-sampled label used for model 2 is better. It's recall is better than the performance of model 1, using the original dataset. 
It correctly classified '1 high-risk loans' at 99% compared to model 1 which classified at 91%. 
The company's is more interested in predicting borrowers that will default, so it can define the appropraite clauses in the lending contract e.g interest rates, duration of loan etc

So I recommend using the model 2. As the company continues to collect data, the distribution of the loan status (data label) will be widely skewed to more '0 healthy loans',
this will degrade model 1 performance.
However, with over-sampling the data (label) the skewed distribution will not degrade the model performance. 


