# Predicting-House-prices-from-Melbourne-housing-dataset-using-R

**Project Overview** <br>
The project aims to identify and prioritize critical decision variables in property investment using multiple linear regression. It assesses how different features, especially property type and regional location, influence the price of properties in Melbourne.

**Data Description:** <br>
Dataset: Melbourne housing with 13,580 observations and 21 variables.<br>
Study Focus: Impact of "Type" and "Region name" on property investment analysis.<br>
Selected Features: Price, Bathroom, Room, YearBuilt, Distance, Landsize, Type, Regionname.<br>
Outliers and Abnormalities: Removed after visual inspection (e.g., YearBuilt = 1196, Landsize = 37000).<br>
Final Dataset: 8,205 observations after removing outliers and null values.

**Analysis Planning:** <br>
Models: Three models constructed to evaluate "Region name" and "Type."<br>
Assumptions: Quantitative/categorical predictors, continuous outcome, non-zero variance, no perfect multicollinearity, predictors uncorrelated with external variables, normal/homoscedastic/independent residuals.

**Results:** <br>
Model Performance: Measured using R-squared, Durbin-Watson Test, Cook’s Distance, VIF.<br>
Key Findings: <br>
- Model with "Region name" is more ideal than with "Type."<br>
- No influential points or collinearity detected.<br>
- Residual analysis shows non-normality and non-homoscedasticity.<br>
ANOVA Test: Revealed that both "Type" and "Region name" significantly improve model performance over the baseline.

**Coefficients (Model with Region name):** <br>
Significant predictors include Rooms, YearBuilt, Bathroom, Landsize, Distance, and various "Region name" categories. <br>
The model accounts for 59% of the variation in house prices.

**Conclusion:** <br>
"Region name" is a better predictor than "Type."<br>
Including both features improves model performance.<br>
The model has limitations due to violated assumptions and may not generalize well for price predictions.

**Managerial Implications:** <br>
The analysis aids in understanding factors influencing property prices.<br>
Provides a basis for forecasting the impact of specific features on house prices.
