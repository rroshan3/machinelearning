# Using Machine Learning and Neural Networks to Determine Highest Impact Factors for Household Income and Wealth

This project compares and contrasts the determinants of household income and household wealth using the Panel Study of Income Dynamics (PSID). 


## Data And Variables Used

PSID public microdata (Excel extract J353982.xlsx) was used with a codebook and a labels text file. 
We analyzed family income in 1984, 1989, 1994, 2006, 2014, 2022 and family wealth in 1984, 1989, 1994, 2005, 2013, 2023. Covariates include Head age, sex, race, family size, employment now, and own/rent.



## Methodology Used

We used waves spanning yr_min to yr_max, harmonized variable names with the provided labels file, and reshaped the data to a person-year panel that is comparable across time. We modeled income and wealth as functions of demographic and family characteristics with year fixed effects, then visualized long-run trends. The models used here were LASSO, Random Forest, Neural Network, and OLS, which we used as the baseline model. We used a permutation test to determine income differences by sex of head and neural network feature importance.


## Summary of Findings

Time trend: household log income rises over calendar years and newer decades

Head characteristics:
Older heads tend to have higher incomes
Sex and race categories show systematic differences in expected income

Household structure:
Tenure and employment status are important predictors in all models

Model comparison:
Neural network provides best performance
OLS and LASSO provide similar performance to neural network model
Random Forest is less accurate but agrees on which predictors matter
