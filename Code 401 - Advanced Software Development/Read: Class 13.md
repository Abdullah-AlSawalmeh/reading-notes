# About Linear Regression
- linear regression is a popular technique and you might as well seen the mathematical equation of linear regression.

- There are several ways in which you can do that, you can do linear regression using numpy, scipy, stats model and sckit learn


## Scikit-learn 
- is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction.


- If you want to look inside the linear regression object, you can do so by typing LinearRegression. and the press <tab> key. This will give a list of functions available inside linear regression object.



## Important functions while fitting a linear regression model are:

1) lm.fit() -> fits a linear model

2) lm.predict() -> Predict Y using the linear model with estimated coefficients

3) lm.score() -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.

## Residual Plots
- Residual plots are a good way to visualize the errors in your data. If you have done a good job then your data should be randomly scattered around line zero. If you see structure in your data, that means your model is not capturing some thing.

![](https://d2mvzyuse3lwjc.cloudfront.net/doc/en/UserGuide/images/Graphic_Residual_Analysis/Graphic_Residual_Analysis-3.jpg?v=10730)

## More about Linear Regression type
Simple linear regression 1 dependent variable (interval or ratio), 1 independent variable (interval or ratio or dichotomous)

- Multiple linear regression 1 dependent variable (interval or ratio) , 2+ independent variables (interval or ratio or dichotomous)

- Logistic regression 1 dependent variable (dichotomous), 2+ independent variable(s) (interval or ratio or dichotomous)

- Ordinal regression 1 dependent variable (ordinal), 1+ independent variable(s) (nominal or dichotomous)


