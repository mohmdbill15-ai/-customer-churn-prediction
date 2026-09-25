# Customer Churn Prediction 
 
## Week 1: Exploratory Data Analysis 
 
### Dataset - Source: Telco Customer Churn (Kaggle) - Size: 7,043 customers, 21 features - Target: Predict customer churn (Yes/No) 
 
### Key Findings 
-Customers with shorter tenure appear more likely to churn than long-term customers.
-Monthly charges show a noticeable relationship with churn, with higher-paying customers appearing more likely to leave.
-Customers on month-to-month contracts show higher churn compared with customers on longer-term contracts.
-Internet service type and payment method show different churn patterns across customer groups.
-The analysis suggests that tenure, contract type, charges, services, and payment method may be useful features for predicting customer churn.
 
### Setup 
Open the Kaggle notebook or run locally: 
pip install pandas numpy matplotlib seaborn

## Week 2: Building ML Models
- Baseline (always "stay"): accuracy [X]
- Best model: [name], AUC [X], recall [X] at threshold [t]
- Top churn drivers (permutation importance): [feature 1], [2], [3]
- Threshold chosen: [t], because [business reason]
- Engineered features: [names]; effect on AUC: [before -> after]
-  Biggest lesson: [one sentence]
