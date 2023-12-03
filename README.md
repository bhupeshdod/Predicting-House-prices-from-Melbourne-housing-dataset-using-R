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

| Test/Model          | Model without Type and Regionname | Model with Type | Model with Regionname |
|-----------------|:--------------------:|:---------------:|:---------------:|
| Multiple R-squared  |              0.4986               |     0.5202      |        0.5963         |
| Durbin-Watson Test  |            1.4774, p=0            |   1.369, p=0    |      1.6834, p=0      |
| Max Cook's Distance |              0.0097               |     0.0115      |        0.0159         |
| Max VIF             |               1.784               |      1.498      |         1.364         |
| Min 1/VIF           |              0.5605               |     0.6674      |        0.7331         |
| Residual Outliers   |                361                |       343       |          330          |

**Coefficients (Model with Region name):** <br>
Significant predictors include Rooms, YearBuilt, Bathroom, Landsize, Distance, and various "Region name" categories. <br>
The model accounts for 59% of the variation in house prices.

**Conclusion:** <br>
"Region name" is a better predictor than "Type."<br>
Including both features improves model performance.<br>
The model has limitations due to violated assumptions and may not generalize well for price predictions.

![image](https://github.com/bhupeshdod/Predicting-House-prices-from-Melbourne-housing-dataset-using-R/assets/141383468/d9944224-318a-4171-89cf-ad4b89f779ff)

**Managerial Implications:** <br>
The analysis aids in understanding factors influencing property prices.<br>
Provides a basis for forecasting the impact of specific features on house prices.
