# Best Invest

Machine learning application that helps businesses understand where they should invest their money within the organization (i.e. R&D spending, Marketing, Administration, etc.) in order to generate the greatest amount of profit.


## File description

-	`Standard_Method.ipynb` - manual step-by-step backward elimination
-	`Auto_Adjusted_P_R2.ipynb`  - automated backward elimination with p-values and adjusted R squared

## Methodology

Goal is to use backward elimination to optimize the multiple linear (step-wise) regression model in order to see the impact each variable has on the organization’s profit. The five-step process for eliminating variables is listed below (“Backward Elimination Steps”). 

Why eliminate variables? 

-	Reliability – insignificant variables can make predictions less dependable, weakening your model

-	Practicality – especially when working with large datasets, it’s more practical to only keep the important variables for better interpretation and understanding for yourself and others

## Backward Elimination Steps

1.	Select a significance level to stay in the model (i.e. SL = 0.05)

2.	Fit the full model with all possible predictors

3.	Consider the predictor with the highest P-value. if P > SL, go to step 4, otherwise go to FINISH.

4.	Remove the predictor

5.	Fit model again, go back to step 3

FINISH: Model is ready
