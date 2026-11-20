# Credit-Card-Approval

We are trying to predict to whom to approve the credit card.  
Credit score cards are a common risk control method in the financial industry. It uses 
personal information and data submitted by credit card applicants to predict the 
probability of future defaults and credit card borrowings. The bank is able to decide 
whether to issue a credit card to the applicant. Credit scores can objectively quantify 
the magnitude of risk.    
Generally speaking, credit score cards are based on historical 
data. Once encountering large economic fluctuations. Past models may lose their 
original predictive power. Logistic model is a common method for credit scoring.  We 
will be aso using Boosting, Random Forest, and Support Vector Machines to form the 
model and make comparision. Then choosing the best model.    
Our objective is to predict if an applicant is 'good' or 'bad' client. This Machine 
Learning (ML) task is regression since the label (or target) we are trying to predict 
is numeric, we derived it from classifying the given column.  
The example data is provided by Kaggle at [Credit Card 
Approval Prediction](https://www.kaggle.com/datasets/rikdifos/credit-card-approval
prediction?select=application_record.csv).  

## EDA   
There are total of 36457 number of rows and 10 columns.  The target distribution has 
302 number of 1 and 36155 number of 0. Thus, this dataset is highly imbalanced with 
0.8% of 1 and 99.17% of 0. Therefore, we will be doing oversampling to get the 
balanced dataset. There were no missing values except for the 
CNT_FAM_MEMBERS. Then, summary of statistics were calculated. After that target 
variable Analysis was done. And then, categorical value count was done.  

## Feature Engineering    
DAYS_BIRTH Count backwards from current day (0), -1 means yesterday. From this 
column we derived age of the customers as AGE_YEARS  
DAYS_EMPLOYED Count backwards from current day(0). If positive, it means the 
person currently unemployed. From this column we derived 2 other columns no. Of 
employed years as EMPLOYED_YEARS and employee status as IS_EMPLOYED 

<img width="640" height="360" alt="image" src="https://github.com/user-attachments/assets/92206176-127f-4e4b-87e9-9ed4babeb3e6" />

<img width="640" height="360" alt="image" src="https://github.com/user-attachments/assets/b7ff6cc4-e7dc-41e6-b395-ee1815052329" />

<img width="640" height="360" alt="image" src="https://github.com/user-attachments/assets/fbd88bd4-f03f-4d3b-bc91-f45684015a59" />

