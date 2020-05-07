# Credit_card_Default

Problem Statement: Determine client characteristic who are likely to default on their next months credit card payment so that selling cards only to clients who are likely to pay the bills and reduce risk. 

About Dataset
Dataset from UCI Machine Learning Repository:  Default of credit card client dataset

30000 records 
24 attributes 
Predictors:  
Demographic : Age (numeric ), Sex (category). Marriage (category). , Education (category). 
Payments for six months : Pay_0 to Pay_6 (category)
Billed amount for six months: BILL_AMT1 to BILL_AMT6 (numeric)
Payment amount for six months: PAY_AMT1 to PAY_AMT6 (numeric)
Target Variable : Default (category)

Preprocessing
Missing Values: Data does not have missing values
Deleted ID column as it is irrelevant
Created age bins for visualization, not used in modeling
Changed type for categorical variables listed as numeric : Sex, Marriage, Education, Pay_0 to Pay_6 , default
Pay_0 to Pay 6. -1 and -2 are not known assuming these means payment made on time replace -1 and -2 to 0
Education: 5 and 6 are not known, replaced to others
Marriage: 0 is not known, replaced to others
Replaced numbers for names for categorical values: 
Sex: Male , Female
Education: Graduate school ,University, High school, Others
Marriage: Married, Single ,Others 
Default: Yes, No
Outliers were not removed for this analysis

Predictive modeling
This was a classification problem, determining if a client with default on their next credit card statement. 
Split the data into 70% training 30% testing sets
Ran 3 models Logistic Regression, Decision trees and K- Nearest neighbors with k=4.
Accuracy for the models
Logistic Regression :  78%
Decision Tree: 73%
K- Nearest neighbors : 76%

Recommendations
Bank should consider giving cards to clients with the following features: 
Clients with a high school diploma and university degree are likely to default. This may be due to low income paying jobs, unemployment. High student debt for clients with university degree.
Clients in the age range of 25yrs to 35 yrs. are also likely to default. 
Data shows that married couple are likely to default than single clients. 
Bank should also keep a close watch on clients who have a credit card with the above characteristics and take necessary actions to avoid the risk of a client defaulting. 
Further analysis is recommended using dataset with data for more than six months to get better insights. 

