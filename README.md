# Assignment 08 - Regression and Evaluation

This repository contains the machine learning assignment focusing on regression modeling and model evaluation using the California Housing dataset.

## 📌 Project Overview
The objective of this assignment is to build, tune, and evaluate various regression models to predict median house values in California districts. The workflow includes data preprocessing, exploratory data analysis, multi-model implementation, evaluation metrics comparison, and hyperparameter tuning using cross-validation.

## 📊 Dataset
* **Source:** `fetch_california_housing` from `sklearn.datasets`
* **Features:** Median Income, House Age, Average Rooms, Average Bedrooms, Population, Average Occupancy, Latitude, and Longitude.
* **Target Variable:** `MedHouseValue` (Median house value for California districts)

## 🤖 Models Implemented
1. **Linear Regression**
2. **Decision Tree Regressor**
3. **Random Forest Regressor**
4. **Gradient Boosting Regressor**
5. **Support Vector Regressor (SVR)**

## 📈 Evaluation Metrics
All models were evaluated using the following standard regression metrics:
* **Mean Squared Error (MSE)**
* **Mean Absolute Error (MAE)**
* **R-Squared ($R^2$) Score**

## 🔍 Key Results & Findings
* **Best Performing Model:** **Random Forest Regressor** achieved the highest performance with the lowest MSE/MAE and an $R^2$ score of approximately **0.805**, explaining ~80.5% of the variance in housing prices.
* **Ensemble Superiority:** Ensemble methods (Random Forest and Gradient Boosting) significantly outperformed linear and support vector approaches due to the non-linear nature of the housing data.
* **Hyperparameter Tuning:** Using `RandomizedSearchCV` with 5-fold cross-validation (`cv=5`) optimized the Random Forest hyperparameters (`n_estimators: 200`, `max_depth: 20`, `min_samples_split: 2`), yielding a robust Cross-Validation $R^2$ score of **~0.805**.

## 🛠️ Requirements & Libraries
* Python 3.x
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
