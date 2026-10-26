# Used-Car Price Prediction

## Project Overview

This project uses machine learning to predict the asking prices of used cars based on selected vehicle characteristics. It was developed as part of a Data Science Capstone Project to apply data cleaning, exploratory data analysis, feature preparation, regression modelling, model evaluation and error analysis.

## Problem Statement

Used-car prices vary according to factors such as brand, model, year, vehicle age, mileage, transmission type, previous ownership and fuel type. The goal of this project is to investigate these features and develop a model that can estimate a used car's asking price.

## Dataset

The dataset contains used-car listings. The data preparation process included:

- Removing duplicate records.
- Cleaning and converting asking prices and mileage into numeric values.
- Investigating invalid or unusual year values.
- Handling missing values.
- Preparing categorical and numerical features for modelling.

After duplicate removal, the dataset contained 14,988 records.

## Features Used

The final model uses eight predictors:

- Brand
- Model
- Year
- Age
- Kilometres driven
- Transmission
- Previous owner
- Fuel type

The target variable is the asking price (`AskPrice_Numeric`).

## Methodology

The project followed these stages:

1. Data loading and exploration.
2. Data cleaning and missing-value handling.
3. Feature selection and preparation.
4. Encoding categorical variables.
5. Splitting the data into training and testing sets.
6. Training and evaluating Linear Regression and Random Forest regression models.
7. Hyperparameter tuning using RandomizedSearchCV.
8. Error analysis and interpretation of model performance.

The dataset was split into 80% training data and 20% testing data.

## Model Results

The following results were obtained during model evaluation:

| Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MAE | ₹631,532.54 | ₹253,924.98 |
| RMSE | ₹1,443,698.86 | ₹842,636.13 |
| R² | 0.2814 | 0.7552 |

Random Forest performed better than Linear Regression on the test set across the reported metrics.

Hyperparameter tuning was also attempted. It did not improve the reported test-set performance, indicating that further experimentation may be needed.

## Key Findings

- Random Forest provided stronger predictive performance than Linear Regression.
- Prediction errors varied across vehicle price ranges.
- More expensive vehicles were associated with larger absolute prediction errors.
- Further work could improve feature engineering, investigate unusual price values and test the model on newer listings.

## Limitations

The predictions depend on the quality and representativeness of the dataset. Missing-value treatment, unusual observations and variation in vehicle prices may affect accuracy. The model should not be treated as a guaranteed market valuation.

## Future Improvements

- Explore additional vehicle features.
- Investigate outliers and unusual prices.
- Experiment with alternative models and feature engineering.
- Validate predictions using newer used-car listings.
- Consider developing an interactive Streamlit application if required.

## Tools and Technologies

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib and Seaborn
- scikit-learn
- GitHub

## Project Status

The notebook is being checked to ensure that the cells run correctly from beginning to end. The presentation and repository documentation are being prepared.

## Author

**Unathi Ndongeni**

Data Science Capstone Project
