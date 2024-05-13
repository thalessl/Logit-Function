This function conducts logistic regression analysis with optional heteroscedasticity correction, VIF calculation, and correlation matrix computation. The function takes as inputs a dependent variable, a list of independent variables, and a dataset. By default, it assumes clustering by a specified variable (default: "COUNTRYCODE"). It first constructs a logistic regression formula and fits the model using the rms package. If heteroscedasticity is detected (using the Breusch-Pagan test), it corrects for it using robust standard errors. It then calculates VIF values to check for multicollinearity and computes a correlation matrix. Additionally, it extracts coefficients, variance-covariance matrix, and computes log-odds ratios with confidence intervals. Finally, it saves the fitted model and results as RDS files and returns them for further analysis.





