# Car Price Prediction Using Machine Learning

## Project Overview

This project develops machine learning regression models to predict automobile prices based on vehicle specifications and characteristics.

The analysis is based on an automobile dataset containing various technical and categorical features of cars. The objective is to identify the key factors influencing car prices and build models that can accurately predict prices.

## Business Objective

A Chinese automobile company plans to enter the US automobile market and manufacture cars locally. This project aims to provide data-driven insights into the factors associated with automobile prices and support pricing and market-entry decisions.

## Dataset

The dataset contains **205 automobile records and 26 columns**, including features related to:

* Engine size
* Horsepower
* Curb weight
* Car dimensions
* Fuel type
* Body style
* Drive type
* Highway MPG
* City MPG
* Car brand
* Price

The `car_ID` identifier was removed, and the car brand was extracted from the `CarName` feature.

## Data Preprocessing

The following preprocessing steps were performed:

* Checked for missing values and duplicate records
* Removed the identifier column
* Extracted automobile brand information
* Separated features and target variable
* Identified numerical and categorical features
* Applied StandardScaler to numerical features
* Applied OneHotEncoder to categorical features
* Created a preprocessing pipeline
* Split the dataset into training and testing sets using an 80:20 ratio

## Machine Learning Models

Five regression algorithms were implemented and evaluated:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor
5. Support Vector Regressor (SVR)

The models were evaluated using:

* R² Score
* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)

## Model Performance

The Random Forest Regressor achieved the strongest performance among the baseline models, with an R² score of approximately **0.96** on the test set.

Hyperparameter tuning was also performed using **GridSearchCV with 5-fold cross-validation** to evaluate whether tuning could further improve the Random Forest model.

## Feature Importance

Random Forest feature importance analysis identified **engine size** and **curb weight** as the most influential features used by the model for predicting automobile prices.

Other relatively important features included highway MPG and horsepower.

These results indicate that vehicle specifications play an important role in the model's price predictions.

## Business Insights

The analysis provides useful insights into the relationship between vehicle characteristics and automobile prices.

The findings can help the automobile company understand pricing patterns in the US automobile market and support further analysis of vehicle specifications and pricing strategies.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Files

* `Car_Price_Prediction.ipynb` — Complete data analysis and machine learning implementation
* `CarPrice_Assignment.csv` — Dataset used for the project

## Conclusion

This project demonstrates the application of machine learning regression techniques to an automobile pricing problem. The models, evaluation metrics, feature importance analysis, and hyperparameter tuning provide a structured approach to understanding and predicting automobile prices from vehicle characteristics.
