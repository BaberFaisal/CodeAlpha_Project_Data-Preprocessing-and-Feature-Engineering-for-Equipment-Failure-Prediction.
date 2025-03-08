# CodeAlpha_Project_Data-Preprocessing-and-Feature-Engineering-for-Equipment-Failure-Prediction.
# Data Preprocessing and Feature Engineering for Equipment Failure Prediction

## Overview
This project focuses on preprocessing and feature engineering for a dataset related to equipment failure prediction. The goal is to clean the data, handle missing values and outliers, engineer new features, normalize the dataset, and balance the classes to improve machine learning model performance.

## Steps Performed

### 1. Data Cleaning
- Removed irrelevant columns (`UDI`, `Product ID`).
- Encoded categorical variables (`Type`) using **Label Encoding**.

### 2. Handling Outliers
- Used the **Interquartile Range (IQR) method** to remove extreme values in numerical features.

### 3. Feature Scaling
- Standardized numerical features using **StandardScaler**.

### 4. Feature Engineering
- Added **rolling statistics** (mean, standard deviation) for `Torque [Nm]`.
- Created **polynomial interaction features** to capture nonlinear relationships.
- Removed highly correlated features to prevent redundancy.

### 5. Data Splitting
- Split the dataset into **training (80%) and testing (20%)** sets.

### 6. Handling Class Imbalance
- Used **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset.

### 7. Feature Selection
- Applied **Random Forest** to determine feature importance.
- Retained only the most relevant features using **SelectFromModel**.

## Files Generated
- `X_train.csv`, `X_test.csv`: Preprocessed training and testing feature datasets.
- `y_train.csv`, `y_test.csv`: Corresponding labels for machine failure prediction.

## Dependencies
- Python 3.7+
- pandas
- scikit-learn
- imbalanced-learn
- numpy

## How to Run
1. Ensure all dependencies are installed (`pip install pandas scikit-learn imbalanced-learn numpy`).
2. Place the dataset (`ai4i2020.csv`) in the working directory.
3. Run the preprocessing script.
4. Use the output files for model training.

## Next Steps
- Train machine learning models using the preprocessed dataset.
- Optimize hyperparameters for better predictions.
- Explore deep learning techniques for further improvement.


