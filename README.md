# Car Price Prediction Using Multiple Linear Regression

**Author**: Sukanna Das  
**Class**: MSCDSA  
**Registration No**: 23122039  

## Project Overview

This project builds a Multiple Linear Regression (MLR) model to predict car prices based on key features. Using a dataset of various car attributes, the model aims to determine how certain features influence car prices.

## Dataset

The dataset (`cardata.csv`) includes the following columns:

- **Car_Name**: Car model name
- **Year**: Year of manufacture
- **Selling_Price**: Price at which the car was sold
- **Present_Price**: Original showroom price when new
- **Kms_Driven**: Total kilometers driven by the car
- **Fuel_Type**: Fuel type (Petrol, Diesel, CNG)
- **Seller_Type**: Seller type (Dealer or Individual)
- **Transmission**: Transmission type (Manual or Automatic)
- **Owner**: Number of previous owners

## Project Steps

### 1. Data Preprocessing

- Loaded libraries (`pandas`, `matplotlib.pyplot`, `seaborn`, `scikit-learn`)
- Checked for null values, data types, and overall dataset shape
- Converted categorical variables (`Fuel_Type`, `Seller_Type`, `Transmission`) into numerical values for modeling

### 2. Data Visualization

- **Correlation Heatmap**: Displayed relationships between features to understand which ones correlate with `Selling_Price`
- **Scatter Plot**: Visualized the relationship between `Selling_Price` and `Present_Price`

### 3. Model Building and Evaluation

#### Lasso Regression
- Identified key features (`Year`, `Present_Price`) by setting irrelevant feature coefficients to zero
- Calculated R-squared error for model evaluation: **0.8436**

#### Multiple Linear Regression
- Trained the model using `Year` and `Present_Price` as predictor variables
- Evaluation metrics:
  - **Mean Absolute Error (MAE)**: 1.239
  - **Mean Squared Error (MSE)**: 2.741
  - **R-squared Error**: 0.8496

### 4. Results Summary

- **MAE**: Average deviation from actual prices is approximately 1.239
- **MSE**: Average squared error is around 2.741
- **R-squared**: Model explains around 85% of the variance in car prices

## Files in Repository

- **cardata.csv**: Dataset
- **MLR_Car_Price_Prediction.ipynb**: Notebook with code and analysis
- **README.md**: Project overview


