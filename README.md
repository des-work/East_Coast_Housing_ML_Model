
# Real Estate Analysis Project - README

## Project Overview

The Real Estate Analysis project aims to investigate the relationship between real estate metrics and weather data. The project includes loading and analyzing housing data, preprocessing, exploratory data analysis, and building regression models.

## Key Changes and Enhancements

### 1. Data Loading and Exploration:

- Loaded housing data from an SQLite database using SQLAlchemy.
- Explored and printed the queried data.
- Calculated and visualized the correlation matrix between features.

### 2. Data Preprocessing:

- Removed outliers from the 'price' column using the Interquartile Range (IQR) method.
- Selected relevant features ('house_size', 'zip_code', 'acre_lot', 'bed') for building regression models.
- Split the data into training and testing sets.
- Standardized features using StandardScaler.
- Applied Principal Component Analysis (PCA) for dimensionality reduction.
- Utilized K-Means Clustering for grouping data.

### 3. Regression Models:

- Implemented various regression models: Linear Regression, Decision Tree Regressor, Random Forest Regressor, and Gradient Boosting Regressor.
- Cross-validated the models using R-squared as the evaluation metric.
- Determined the best model based on the minimum R-squared error.

### 4. Hyperparameter Tuning:

- Conducted hyperparameter tuning for the Random Forest Regressor using GridSearchCV.
- Trained the Random Forest model with the best hyperparameters.

### 5. Feature Importance:

- Extracted feature importances from the trained Random Forest model.
- Created and printed a DataFrame to display feature importances.
- Visualized feature importances using a bar chart.

### 6. Visualizations:

- Improved the visualization of the PCA and Clustering results.
- Enhanced the visualization of the Feature Correlation Matrix using a heatmap.

### 7. Model Results:

#### Linear Regression
- Cross-Validated R Squared Error: -0.09838708376026908

#### Decision Tree Regressor
- Cross-Validated R Squared Error: -0.9543269180905426

#### Random Forest Regressor
- Cross-Validated R Squared Error: -0.9650023979091239

#### Gradient Boosting Regressor
- Cross-Validated R Squared Error: -0.706194625056925

**Best Model: Random Forest Regressor**

#### Optimized Model Results:
# Optimized Model Results

## Mean Squared Error (MSE): 678,438,335.48

The Mean Squared Error (MSE) is a measure of the average squared difference between predicted and actual values. In this optimized model, the MSE is approximately 678 million, indicating the average magnitude of errors in the predicted housing prices.

## R-squared (R²): 0.984

The R-squared value, also known as the coefficient of determination, represents the proportion of the variance in the dependent variable (housing prices) that is predictable from the independent variables (features). A value of 0.984 indicates an excellent fit, suggesting that 98.4% of the variance in housing prices is explained by the model.

## Feature Importances

The feature importances provide insights into the contribution of each feature to the model's predictions. Here are the top features:

1. **house_size (42.46%)**: The size of the house is the most influential feature, contributing 42.46% to the model's predictive power.

2. **zip_code (41.01%)**: The zip code of the property is another crucial factor, contributing 41.01% to the model.

3. **acre_lot (12.40%)**: The size of the land (acreage) has a notable impact, accounting for 12.40% of the predictive power.

4. **bed (4.13%)**: The number of bedrooms also contributes, although to a lesser extent (4.13%).

## Conclusion

The optimized model performs exceptionally well, with a high R-squared value and relatively low MSE. The top features, 'house_size' and 'zip_code,' are key drivers of housing prices, highlighting the significance of both the property's size and its location.

The results affirm the effectiveness of the regression model in capturing the relationships between features and housing prices. The low MSE indicates accurate predictions, while the high R-squared suggests a robust fit to the data.

In practical terms, these findings imply that buyers and sellers can use the model to make more informed decisions regarding housing prices based on essential features such as house size, location (zip code), and acreage.

### 8. Summary:

The optimized Random Forest Regressor produced a Cross-Validated R Squared Error of -0.9650023979091239, indicating strong predictive performance. The hyperparameters {'max_depth': None, 'min_samples_leaf': 1, 'min_samples_split': 2, 'n_estimators': 100} were identified as optimal.

The feature importances suggest that 'house_size' and 'zip_code' are the most influential factors in predicting housing prices. The negative correlation between 'zip_code' and 'house_size' may require further investigation, possibly indicating regional variations in house sizes.

In conclusion, the project successfully built regression models, optimized the Random Forest model, and provided insights into feature importance. The results highlight the importance of 'house_size' and 'zip_code' in predicting housing prices.

---

Feel free to adjust the summary section based on additional insights or specific findings from your analysis.
