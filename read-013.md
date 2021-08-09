# Read 13: Linear Regressions:

## How to run Linear regression in Python Scikit-learn?

* **Regression analysis** is one of the most important fields in statistics and machine learning. There are many regression methods available. Linear regression is one of them.

* **Regression** searches for relationships among variables.

* **Linear regression** is a basic and commonly used type of predictive analysis.The overall idea of regression is to examine two things:

  * Does a set of predictor variables do a good job in predicting an outcome (dependent) variable?
  
  * Which variables in particular are ignificant predictors of the outcome variable, and in what way do they–indicated by the magnitude sign of the beta estimates–impact the outcome variable?
    
* **Scikit-learn** is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction.

* If you want to implement linear regression and need the functionality beyond the scope of scikit-learn, you should consider statsmodels. It’s a powerful Python package for the estimation of statistical models, performing tests, and more. It’s open source as well.

* In this section we're going to fit a linear regression model and predict the Boston housing prices. We will use the least squares method as the way to estimate the coefficients: **Y** = boston housing price(also called “target” data in Python) & **X** = all the other features (or independent variables).
