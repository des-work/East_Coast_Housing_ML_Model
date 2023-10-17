# US East Coast Weather & Housing Prices Predictive Modeling

## Overview:

This project aims to uncover insights into the relationship between weather conditions and housing prices in the United States. Leveraging datasets from [Kaggle](https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset/data) and the [OpenWeather API](https://openweathermap.org/api), we employ machine learning techniques to predict and understand the impact of weather on real estate values.

## Key Features:

- **Data Sources:**
  - [USA Real Estate Data](https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset/data): CSV format, covering real estate details across the USA.
  - [OpenWeather API](https://openweathermap.org/api): Providing temperature, humidity, and precipitation data.

Certainly! Here's an extended section with the results from the Correlation Matrix Analysis:

# Real Estate and Weather Data Analysis

## Authors:
* Desmond Workman
* [Author 2]

## Date: 10/19/2023

### Overview
This project explores the correlation between real estate metrics and weather data. 

###Local Models
* Import data models and libraries.
* Merge datasets based on a common feature.
* Evaluate data correlations and drop unnecessary columns.
* Remove outliers from the price column.
* Split the data into training and testing sets.
* Standardize features and apply Principal Component Analysis (PCA) for dimensionality reduction.
* Apply K-Means Clustering with three clusters.
* Implement various regression models and cross-validate their performance.
* Perform hyperparameter tuning on the Random Forest Regressor.
* Train the best model using the tuned parameters.
* Analyze feature importances and visualize results.
* Conduct a Correlation Matrix Analysis.

### Data Sources and Sessions
* Utilize local models and sessions for data retrieval.
* Load real estate and weather data from CSV files.
* Merge datasets based on a common feature.
* Close sessions after data retrieval.

### Data Preprocessing
* Load real estate and weather data from CSV files.
* Merge datasets based on a common feature.
* Drop unnecessary columns and evaluate data correlations.
* Remove outliers from the price column.
* Split the data into training and testing sets.
* Standardize features and apply PCA for dimensionality reduction.
* Apply K-Means Clustering with three clusters.

### Correlation Matrix Analysis

#### Results:
The correlation matrix analysis reveals the following strong positive and negative correlations between variables:

| Variable           | Strong Positive Correlations                 | Strong Negative Correlations                 |
|--------------------|----------------------------------------------|----------------------------------------------|
| Unnamed: 0         | Zip Code (0.659092)                          | -                                            |
| Bed                | Bath (0.648341), House Size (0.479547)       | -                                            |
| Bath               | Bed (0.648341), House Size (0.524287)        | -                                            |
| Acre Lot           | -                                            | -                                            |
| Zip Code           | Unnamed: 0 (0.659092)                        | House Size (-0.031749)                       |
| House Size         | Bed (0.479547), Bath (0.524287)              | Zip Code (-0.031749)                         |
| Price              | Bath (0.567940), House Size (0.349971), Price Per Sqfoot (0.684290) | -                     |
| Price Per Sqfoot   | Price (0.684290)                             | -                                            |

### Regression Models
* Implement various regression models: Linear Regression, Decision Tree Regressor, Random Forest Regressor, Gradient Boosting Regressor.
* Cross-validate each model's performance.
* Perform hyperparameter tuning on the Random Forest Regressor.
* Train the best model using the tuned parameters.

### Feature Importances
* Analyze feature importances of the best Random Forest model.
* Create and display a dataframe with feature importances.
* Visualize feature importances through a bar plot.

### Clustering Visualization
* Visualize clustering results using PCA.

### Best Model Selection
* Identify the best-performing model based on cross-validated mean squared error.

### Conclusion
* Summarize findings, explain biases and limitations, and suggest potential improvements.

This README now includes a detailed section with the results from the Correlation Matrix Analysis.

By following these steps, users can explore the intricate relationships between weather conditions and housing prices in the US.

---

Feel free to customize the README further based on specific details and results from your project.
