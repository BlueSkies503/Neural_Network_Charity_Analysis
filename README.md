# Neural_Network_Charity_Analysis

## Overview
The goal of this project is to use features in the provided dataset to create a binary classifier that will predict whether or not applicants will be successful if funded.

## Results
- Data Preprocessing
	- Target variable: 'IS_SUCCESSFUL' column. 
	- Model Features: ['STATUS', 'ASK_AMT', 'APPLICATION_TYPE_Other', 'APPLICATION_TYPE_T10',
       'APPLICATION_TYPE_T19', 'APPLICATION_TYPE_T3', 'APPLICATION_TYPE_T4',
       'APPLICATION_TYPE_T5', 'APPLICATION_TYPE_T6', 'APPLICATION_TYPE_T7',
       'APPLICATION_TYPE_T8', 'AFFILIATION_CompanySponsored',
       'AFFILIATION_Family/Parent', 'AFFILIATION_Independent',
       'AFFILIATION_National', 'AFFILIATION_Other', 'AFFILIATION_Regional',
       'CLASSIFICATION_C1000', 'CLASSIFICATION_C1200', 'CLASSIFICATION_C2000',
       'CLASSIFICATION_C2100', 'CLASSIFICATION_C3000', 'CLASSIFICATION_Other',
       'USE_CASE_CommunityServ', 'USE_CASE_Heathcare', 'USE_CASE_Other',
       'USE_CASE_Preservation', 'USE_CASE_ProductDev',
       'ORGANIZATION_Association', 'ORGANIZATION_Co-operative',
       'ORGANIZATION_Corporation', 'ORGANIZATION_Trust', 'INCOME_AMT_0',
       'INCOME_AMT_1-9999', 'INCOME_AMT_10000-24999',
       'INCOME_AMT_100000-499999', 'INCOME_AMT_10M-50M', 'INCOME_AMT_1M-5M',
       'INCOME_AMT_25000-99999', 'INCOME_AMT_50M+', 'INCOME_AMT_5M-10M',
       'SPECIAL_CONSIDERATIONS_N', 'SPECIAL_CONSIDERATIONS_Y']
	- Variables that need removal: 'EIN' and 'NAME'
- Compiling, Training, and Evaluating the Model
	- Neurons: 210, layers: 3, activation function: sigmoid
	- Achieve target model performance? No, attempts achieved only up to 72% accuracy.
	- What steps did you take to try and increase model performance?
#### Optimization
Attempts:
1.	- 100 Epochs
	- Hidden Layer 1: 80
	- Hidden Layer 2: 30
	- Activation: Sigmoid
	- Accuracy 0.7262973785400391 
2.	- 500 Epochs
	- Hidden Layer 1: 80
	- Hidden Layer 2: 30
	- Activation: Sigmoid
	- Accuracy 0.7243148684501648
3.	- 500 epochs
	- Hidden Layer 1: 120
	- Hidden Layer 2: 70
	- Activation: Sigmoid
	- Accuracy: 0.7257142663002014
4.	- 500 epochs
	- Hidden Layer 1: 120
	- Hidden Layer 2: 70
	- Activation: ReLu
	- Accuracy: 0.46682214736938477
5.	- 500 Epochs
	- Hidden Layer 1: 120
	- Hidden Layer 2: 70
	- Hidden Layer 3: 20
	- Activation: Sigmoid
	- Accuracy: 0.7255976796150208

## Summary
Final accuracy was about 72%, more work could be explored with different activation functions, or trying to drop some of the variables. Although it is not clear which variables are crucial data.
