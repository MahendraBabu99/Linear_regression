Linear Regression on California Housing Dataset

This repository contains an end-to-end implementation of a Linear Regression model using scikit-learn to predict median house prices based on socioeconomic and geographic features from the California Housing dataset.

📌 Overview

The project focuses on building a clean and reproducible regression pipeline that includes data preprocessing, model training, and evaluation. The target variable (MedHouseVal) is continuous, making it a suitable use case for linear regression.

🗂 Dataset

Source: sklearn.datasets.fetch_california_housing

Target variable: Median house value (MedHouseVal)

Features: Numerical attributes such as median income, average rooms, population, housing age, and location-based metrics

⚙️ Preprocessing

Data preprocessing is handled using Pipeline and ColumnTransformer to ensure modularity and prevent data leakage:

Missing numerical values are handled using mean imputation

Features are scaled using StandardScaler

The preprocessing steps are fully integrated into the model pipeline

🧠 Model

Algorithm: Linear Regression

Train–Test Split: 80% training, 20% testing

The model is trained using scikit-learn’s LinearRegression estimator

📊 Evaluation Metrics

Model performance is evaluated using standard regression metrics:

R² Score – Measures the proportion of variance explained by the model

Mean Absolute Error (MAE) – Average absolute difference between actual and predicted values

Root Mean Squared Error (RMSE) – Penalizes larger prediction errors

These metrics provide a comprehensive view of both accuracy and error behavior.

✅ Results

The baseline Linear Regression model achieves a reasonable performance, explaining a significant portion of variance in house prices. This serves as a strong foundation for experimenting with advanced techniques such as regularization (Ridge, Lasso) or non-linear models.

🚀 Future Improvements

Add Ridge and Lasso regression for regularization

Perform feature importance analysis

Visualize residuals and prediction errors

Compare performance with tree-based regressors

📦 Technologies Used

Python

pandas

scikit-learn
