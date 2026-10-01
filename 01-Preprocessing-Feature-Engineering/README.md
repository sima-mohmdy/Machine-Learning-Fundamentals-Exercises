
# Preprocessing & Feature Engineering

This folder contains four machine learning exercises focused on **data preprocessing, data cleaning, feature engineering, encoding, discretization, and feature selection**.

The exercises use different real-world datasets and compare the effect of preprocessing and feature engineering on machine learning performance.

## Exercises

### 1. Missing and Outlier Data

**Dataset:** GPS Travel Dataset

Topics covered:

* Handling missing values
* Mean imputation
* Predictive imputation using AutoML
* Missing-value classification
* Outlier detection using the IQR method
* Outlier replacement
* Data visualization with boxplots

---

### 2. Bank Marketing

**Dataset:** Bank Marketing Dataset

Topics covered:

* Identifying missing values represented by `unknown`
* Mode imputation for categorical features
* Binary encoding
* One-hot encoding
* Ordinal encoding
* Identifying categorical, continuous, binary, nominal, and ordinal features
* Comparing model performance before and after preprocessing

---

### 3. Urban Traffic

**Dataset:** Urban Traffic Dataset

Topics covered:

* Date and time feature engineering
* Gregorian to Jalali date conversion
* Time discretization
* Holiday feature creation
* Seasonal feature creation
* One-hot encoding
* Comparing model performance before and after feature engineering

---

### 4. Tsubasa

**Dataset:** Football Shot Dataset

Topics covered:

* Creating a binary target variable
* Removing irrelevant features
* Feature engineering from geometric information
* Calculating shot distance and angle
* Handling missing categorical values using domain information
* One-hot encoding
* Feature selection using `mutual_info_classif`
* Comparing model performance before and after feature selection

## Main Topics

Across these exercises, the following machine learning preprocessing concepts are practiced:

* Missing Value Handling
* Outlier Detection
* Data Cleaning
* Categorical Encoding
* One-Hot Encoding
* Binary Encoding
* Ordinal Encoding
* Discretization
* Date/Time Feature Engineering
* Feature Creation
* Feature Selection
* Mutual Information
* Data Visualization
* Model Performance Comparison

## Files

```text
01-Preprocessing-Feature-Engineering/
│
├── README.md
├── [Exercise 1 notebook]
├── [Exercise 2 notebook]
├── [Exercise 3 notebook]
└── [Exercise 4 notebook]
```

Each notebook contains the corresponding dataset preprocessing steps, feature engineering techniques, experiments, and model performance comparisons.
