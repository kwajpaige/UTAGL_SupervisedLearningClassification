# UTAGL_SupervisedLearningClassification
Supervised Learning Classification focuses on leveraging data to build ML Classification models which predict classification labels for unseen data.  Focus of this repository is logistic regression and decision trees. 

Link to Jupyter notebook: https://github.com/kwajpaige/UTAGL_SupervisedLearningClassification/blob/main/PaigeSingleton_SupervisedLearningClassificationPersonalLoanCampaign072022.ipynb

## Background
AllLife Bank is a US bank that has a growing customer base. The majority of these customers are liability customers (depositors) with varying sizes of deposits. The number of customers who are also borrowers (asset customers) is quite small, and the bank is interested in expanding this base rapidly to bring in more loan business and in the process, earn more through the interest on loans. In particular, the management wants to explore ways of converting its liability customers to personal loan customers (while retaining them as depositors).

A campaign that the bank ran last year for liability customers showed a healthy conversion rate of over 9% success. This has encouraged the retail marketing department to devise campaigns with better target marketing to increase the success ratio.

## Data Dictionary
- ID: Customer ID
- Age: Customer’s age in completed years
- Experience: #years of professional experience
- Income: Annual income of the customer (in thousand dollars)
- ZIP Code: Home Address ZIP code.
- Family: the Family size of the customer
- CCAvg: Average spending on credit cards per month (in thousand dollars)
- Education: Education Level. 1: Undergrad; 2: Graduate;3: Advanced/Professional
- Mortgage: Value of house mortgage if any. (in thousand dollars)
- Personal_Loan: Did this customer accept the personal loan offered in the last campaign?
- Securities_Account: Does the customer have securities account with the bank?
- CD_Account: Does the customer have a certificate of deposit (CD) account with the bank?
- Online: Do customers use internet banking facilities?
- CreditCard: Does the customer use a credit card issued by any other Bank (excluding All life Bank)?

## Objective
Build a model that will help the marketing department to identify the potential customers who have a higher probability of purchasing the loan.


## Model Performance and Takeaways 
Decision Tree Best Model 2, fit to data set with ccp alpha .01 has a recall on test data of .099 and on train data of .99. Assuming that All Life bank wants loan purchasers to also have a high rate of repayment, use of the recall metric is the best metric to judge madel performance. This indicates that, not only is best_model2, a Decision tree model, is the best model decision tree model, it si also the best of the two options in this project: Logistic Regression and Decision Tree as it gives the highest recall score of all models.

Key takeaways
The key variables that have a strong relatiosnhip to the dependent variable follow: Income_scale 0.636685 Education_2 0.103283 Family_3 0.082412 Family_4 0.079906 CCAvg_log 0.056525 Education_3 0.041189

The segment of customers that should be targeted follow: Higher Income individuals (greater than approximately $150,000/year with Degrees (preferable graduate degrees) and families (married and possibly with children). Individuals should have credit card balances.

 
