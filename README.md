# Customer Churn Prediction 
 
## Week 1: Exploratory Data Analysis 
 
### Dataset - Source: Telco Customer Churn (Kaggle) - Size: 7,043 customers, 21 features - Target: Predict customer churn (Yes/No) 
 
### Key Findings 
-Customers with shorter tenure appear more likely to churn than long-term customers.
-Monthly charges show a noticeable relationship with churn, with higher-paying 
  customers appearing more likely to leave.
-Customers on month-to-month contracts show higher churn compared with customers   on longer-term contracts.
-Internet service type and payment method show different churn patterns across  
  customer groups.
-The analysis suggests that tenure, contract type, charges, services, and 
  payment method may be useful features for predicting customer churn.
 
### Setup 
Open the Kaggle notebook or run locally: 
pip install pandas numpy matplotlib seaborn

## Week 2: Building ML Models
Baseline (always "stay"): accuracy 0.735
Best model: Logistic Regression, AUC 0.842, recall 0.567 at threshold 0.50
Top churn drivers (permutation importance): tenure, TotalCharges, Contract_Two year
Threshold chosen: 0.15, because missing a churner costs PKR 6000, compared with PKR 1000 for an unnecessary retention offer
Engineered features: n_services, is_new, charge_per_mo, price_jump; effect on AUC: 0.8422 → 0.8420
Biggest lesson: Lowering the threshold can increase recall when missing a churner is more costly, while the engineered features did not improve Random Forest AUC in this experiment.
