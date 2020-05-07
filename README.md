# Credit_card_Default

Problem Statement: Determine client characteristic who are likely to default on their next months credit card payment so that selling cards only to clients who are likely to pay the bills and reduce risk. 

About Dataset<br />
Dataset from UCI Machine Learning Repository:  Default of credit card client dataset<br />

30000 records<br />
24 attributes<br />
Predictors:<br />
Demographic : Age (numeric ), Sex (category), Marriage (category), Education (category).<br />
Payments for six months : Pay_0 to Pay_6 (category)<br />
Billed amount for six months: BILL_AMT1 to BILL_AMT6 (numeric)<br />
Payment amount for six months: PAY_AMT1 to PAY_AMT6 (numeric)<br />
Target Variable : Default (category)<br />
<br />
Preprocessing<br />
Missing Values: Data does not have missing values<br />
Deleted ID column as it is irrelevant<br />
Created age bins for visualization, not used in modeling<br />
Changed type for categorical variables listed as numeric : Sex, Marriage, Education, Pay_0 to Pay_6 , default<br />
Pay_0 to Pay 6. -1 and -2 are not known assuming these means payment made on time replace -1 and -2 to 0<br />
Education: 5 and 6 are not known, replaced to others<br />
Marriage: 0 is not known, replaced to others<br />
Replaced numbers for names for categorical values:<br /> 
Sex: Male , Female<br />
Education: Graduate school ,University, High school, Others<br />
Marriage: Married, Single ,Others <br />
Default: Yes, No<br />
Outliers were not removed for this analysis<br />

Predictive modeling<br />
This was a classification problem, determining if a client with default on their next credit card statement. <br />
Split the data into 70% training 30% testing sets<br />
Ran 3 models Logistic Regression, Decision trees and K- Nearest neighbors with k=4.<br />
Accuracy for the models<br />
Logistic Regression :  78%<br />
Decision Tree: 73%<br />
K- Nearest neighbors : 76%<br />

Recommendations<br />
Bank should consider giving cards to clients with the following features: <br />
Clients with a high school diploma and university degree are likely to default. This may be due to low income paying jobs, unemployment. High student debt for clients with university degree.<br />
Clients in the age range of 25yrs to 35 yrs. are also likely to default. <br />
Data shows that married couple are likely to default than single clients. <br />
Bank should also keep a close watch on clients who have a credit card with the above characteristics and take necessary actions to avoid the risk of a client defaulting. <br />
Further analysis is recommended using dataset with data for more than six months to get better insights. <br />

