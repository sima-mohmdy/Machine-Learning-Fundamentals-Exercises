# Regression

This folder contains regression projects focused on predicting continuous target variables using different preprocessing techniques, feature engineering methods, feature selection approaches, and regression models.

## Exercises

### 1. Diamond Price Prediction

**Objective:**
Predict diamond prices using their physical and categorical characteristics.

**Dataset:**

* Training set: 50,000 samples
* Test set: 3,940 samples
* Target: `price`

**Main steps:**

* Exploratory inspection of the dataset
* Identification of numerical and categorical features
* Ordinal encoding for `cut` and `clarity`
* One-hot encoding for `color`
* Feature scaling using `StandardScaler`
* Training a `LinearRegression` model
* Evaluation using the R² score
* Generating predictions for the test set and preparing a submission file

**Training R²:** ~88.94%

**Main topics:**

* Linear Regression
* Categorical Encoding
* Ordinal Encoding
* One-Hot Encoding
* Feature Scaling
* R² Evaluation
* Train/Test Preprocessing
* Prediction and Submission

---

### 2. Life Expectancy Prediction

**Objective:**
Predict life expectancy of countries using health, economic, demographic, and development-related indicators.

**Dataset:**

* Training set: 2,848 samples, 22 columns
* Test set: 80 samples, 21 columns
* Target: `Life expectancy`

**Main steps:**

* Exploratory Data Analysis (EDA)
* Statistical analysis and feature inspection
* Missing value detection and handling
* Median imputation for missing numerical values
* Splitting the training data into training and validation sets
* Applying preprocessing consistently across training, validation, and test data
* Label encoding of the `Status` feature
* One-hot encoding of the `Country` feature
* Feature scaling using `MinMaxScaler`
* Feature selection using `SelectKBest` with `f_regression`
* Polynomial feature generation using `PolynomialFeatures`
* Training and comparing regression models:

  * Linear Regression
  * Ridge Regression
  * Lasso Regression
  * ElasticNet
  * Random Forest Regressor
  * Gradient Boosting Regressor
* Hyperparameter tuning for Ridge regularization
* Evaluating models using validation performance
* Generating predictions for the test set and preparing a submission file

**Final Model:**

* Polynomial Features + Ridge Regression

**Validation Performance:**

* **R² Score:** ~96.27%
* **MAE:** ~1.03
* **RMSE:** ~1.83

**Main topics:**

* Regression
* Linear Regression
* Polynomial Feature Generation
* Regularization

  * Ridge Regression (L2 Regularization)
  * Lasso Regression (L1 Regularization)
  * ElasticNet (L1 + L2 Regularization)
* Overfitting Control
* Missing Value Imputation
* Label Encoding
* One-Hot Encoding
* Feature Scaling
* Feature Selection
* Model Comparison
* Hyperparameter Tuning
* R², MAE, RMSE Evaluation
* Train/Validation/Test Preprocessing
* Prediction and Submission Generation

---

## Main Topics Covered

Across these exercises, the following regression concepts and techniques are practiced:

* Regression Algorithms
* Linear Regression
* Polynomial Feature Engineering
* Regularized Regression
* Ridge, Lasso, and ElasticNet
* Feature Selection
* Missing Value Handling
* Categorical Feature Encoding
* Label Encoding
* Ordinal Encoding
* One-Hot Encoding
* Feature Scaling

  * StandardScaler
  * MinMaxScaler
* Model Evaluation

  * R² Score
  * MAE
  * RMSE
* Model Comparison
* Hyperparameter Tuning
* Overfitting Control
* Train/Validation/Test Preprocessing
* Prediction and Submission Generation

## Folder Structure

```text
Regression/
│
├── README.md
│
├── 01-Diamond-Price-Prediction/
│   ├── notebook.ipynb
│   └── data/
│
└── 02-Life-Expectancy-Prediction/
    ├── notebook.ipynb
    └── data/
```
