# Car_price_prediction

# Executive summary
In this project, we will predict what element will affect the price of car. Some questions we want to find the answers:
Do I know if the dealer is offering fair value for my trade-in?
Do I know if I put a fair value on my car?

# Tools using:
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-learn
- Machine Learning

# Methodology

## Data Collection

After importing and reading the data to the csv file, we will do simple data cleaning by adding the header and replacing the missing values. 

## Data Wrangling

- Identify and remove duplicate values
- Identify and impute missing values
- Normalize data

## Data Exploration
- Import Data from the previous module
- Analyzing Individual Features Patterns using Visualization
- Descriptive Statistical Analysis
- Basics of Grouping
- Correlation and Causation
- ANOVA

## Model Development
- Some question we want to ask:
- Do I know if the dealer is offering fair value for my trade-in?
- Do I know if I put a fair value on my car?
- Linear Regression and Multiple Linear Regression
- Model evaluation using visualization (Regression Plot, Residual Plot)
- Polynomial Regression and Pipelines
- Measures for In-sample evaluation (R-square and MSE)
- Prediction and Decision Making

## Model Evaluation and Refinement
- Model Evaluation
- Over-fitting, Under-fitting, and Model Selection
- Ridge Regression
- Grid Search

# Findings:

1. Regression Plot:
From the regression plot, we can see that price is negatively correlated to highway-mpg.

2. Distribution Plot:
One way to look at the fit of the Multiple Linear Regression model is by looking at the distribution plot. After examining the relationship between “price” with “Horsepower”, “Curb-weight”, “Engine-size”, “Highway-mpg”, the result is that the fitted values are reasonably close to the actual values since the two distributions overlap a bit. However, there is definitely some room for improvement.

3. Polynomial Regression:
While performing polynomial model, from the plotting I found that this model performs better than the linear model as the generated polynomial function “hits” more of the data points. 

4. Simple Linear Regression Model (SLR) and Multiple Linear Regression Model (MLR):

In order to compare the results of the MLR vs SLR models, we look at a combination of both the R-squared and MSE to make the best conclusion about the fit of the model.

MSE: The MSE of SLR is  3.16x10^7  while MLR has an MSE of 1.2 x10^7.  The MSE of MLR is much smaller.
R-squared: In this case, we can also see that there is a big difference between the R-squared of the SLR and the R-squared of the MLR. The R-squared for the SLR (~0.497) is very small compared to the R-squared for the MLR (~0.809).

5. Simple Linear Model (SLR) vs. Polynomial Fit:
MSE: We can see that Polynomial Fit brought down the MSE, since this MSE is smaller than the one from the SLR.
R-squared: The R-squared for the Polynomial Fit is larger than the R-squared for the SLR, so the Polynomial Fit also brought up the R-squared quite a bit.
Multiple Linear Regression (MLR) vs. Polynomial Fit:

MSE: The MSE for the MLR is smaller than the MSE for the Polynomial Fit.
R-squared: The R-squared for the MLR is also much larger than for the Polynomial Fit.

6. Comparing three models:
	In conclusion, the MLR model is the best model to be able to predict price from our dataset. This result makes sense since we have 27 variables in total and we know that more than one of those variables are potential predictors of the final car price. 


