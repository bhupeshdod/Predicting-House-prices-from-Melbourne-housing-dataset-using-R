# Predicting-House-prices-from-Melbourne-housing-dataset-using-R

**Overview** <br>
This repository contains a comprehensive analysis of the Melbourne housing market, focusing on determining the impact of various features, including property type and region, on housing prices. The project uses multiple linear regression models to analyze a dataset of 13,580 housing transactions, refined to 8,205 observations after cleaning. The primary goal is to identify key factors influencing property prices, which is crucial for investment analysis and decision-making in the real estate domain.

**Dataset** <br>
The dataset, titled "Melbourne Housing Market," comprises 21 variables and initially includes 13,580 observations. The data covers various aspects of properties sold in Melbourne, such as price, number of bathrooms and rooms, year built, land size, property type, and region. After preprocessing, which involved removing outliers and handling missing values, the dataset was reduced to 8,205 observations.

**Features** <br>
Key features analyzed in the dataset include:
Price: Price of the property in dollars.
Bathroom: Number of bathrooms in the property.
Room: Number of rooms.
YearBuilt: Year in which the property was built.
Distance: Distance from the Central Business District (CBD).
Landsize: Size of the land on which the property is built.
Type: Type of real estate (e.g., house, unit, townhouse).
Regionname: Name of the region where the property is located.

**Assumptions:** <br>
Quantitative/categorical predictors, continuous outcome.
Non-zero variance.
No perfect multicollinearity (verified with VIF test).
Independence from external variables.
Normal, homoscedastic, independent residuals (analysis to follow).

**Key Findings from Tests** <br>
Multiple R-squared: Increases with the inclusion of "Type" and "Region name."
Durbin-Watson Test: Indicates no autocorrelation.
Max Cook’s Distance: Below the cutoff value of 1, indicating no influential outliers.
Max VIF: Well below 10, indicating no multicollinearity.

**Residual Analysis:** <br>
Some non-normality and heteroscedasticity observed in residual plots.
"Region name" model shows better performance compared to the "Type" model.

**ANOVA Test** <br>
Both "Type" and "Region name" models significantly outperform the model without these features.
"Region name" model is superior to "Type" model (F = 407.3, p<0.01).

**Model with Region name - Coefficients** <br>
Significant coefficients for features like Rooms, YearBuilt, Bathroom, Landsize, Distance, and various Region names.
Example: Adding a bathroom increases the price by approximately 180,897.89 to 215,343.25 dollars.

**Conclusion** <br>
"Region name" is a stronger predictor than "Type."
Both features together improve model performance.
The model explains 59% of the variation in house prices.
Certain model assumptions were violated, indicating limitations in generalizability and predictive accuracy.
Residual Analysis: Checking for normality, homoscedasticity, and independence of residuals.
Comparative Analysis: Using ANOVA to compare models.

Key Findings
The feature "Region name" is a stronger predictor of housing prices than "Type."
Including both "Type" and "Region name" enhances the model's predictive power.
The model accounts for approximately 59% of the variation in housing prices.
