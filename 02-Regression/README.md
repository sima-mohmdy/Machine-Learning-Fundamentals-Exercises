
# Regression

This folder contains regression exercises focused on predicting continuous target variables using different preprocessing techniques and regression models.

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
* Feature standardization using `StandardScaler`
* Training a `LinearRegression` model
* Evaluation using the R² score
* Generating predictions for the test set and preparing a submission file

**Training R²:** ~88.94%

**Main topics:**

* Linear Regression
* Categorical Encoding
* Ordinal Encoding
* One-Hot Encoding
* Feature Scaling / Standardization
* R² Evaluation
* Train/Test Preprocessing
* Prediction and Submission

---

### 2. Life Expectancy Prediction

**Objective:**
Predict the life expectancy of countries using health, economic, demographic, and development-related indicators.

**Dataset:**

* Training set: 2,848 samples, 18 columns
* Test set: 80 samples, 17 columns
* Target: `Life expectancy`

**Main steps:**

* Exploratory inspection and statistical analysis
* Detection and analysis of missing values
* Missing-value imputation using the mode
* Applying training-set imputation values consistently to the test set where applicable
* Label encoding of the `Status` feature
* One-hot encoding of the `Country` feature
* Feature scaling using `MinMaxScaler`
* Generating polynomial features using `PolynomialFeatures`
* Training a `LinearRegression` model on polynomial features
* Evaluation using the R² score
* Generating predictions for the test set and preparing a submission file

**Training R²:** ~99.89%

**Main topics:**

* Regression
* Linear Regression
* Polynomial Features
* Polynomial Regression
* Missing Value Handling
* Mode Imputation
* Label Encoding
* One-Hot Encoding
* Feature Scaling / Min-Max Normalization
* R² Evaluation
* Prediction and Submission

---

## Main Topics Covered

Across these exercises, the following regression concepts and techniques are practiced:

* Regression
* Linear Regression
* Polynomial Regression
* Polynomial Feature Generation
* Missing Value Handling
* Categorical Encoding
* Label Encoding
* Ordinal Encoding
* One-Hot Encoding
* Feature Scaling
* Standardization
* Min-Max Normalization
* R² Score
* Train/Test Preprocessing
* Model Training
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
