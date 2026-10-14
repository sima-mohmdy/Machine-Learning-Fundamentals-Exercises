
# Project 1 – Machine Learning Exercises

This project contains two machine learning exercises focused on classification problems, including data preprocessing, feature engineering, model training, and evaluation.

## Exercise 1: Trip Purpose Prediction

**Objective:** Predict the purpose of a trip using the Masterبلیط dataset and the `TripReason` target variable.

### Dataset
- Training data: 101,017 records
- Test data: 43,293 records
- Target variable: `TripReason` (`Work` / `Int`)

### Workflow
- Data preprocessing and missing-value handling
- Removal of unnecessary columns
- Feature engineering and extraction of time-related features
- Categorical feature encoding using `OrdinalEncoder`
- Model training using `RandomForestClassifier` with 100 trees
- Model evaluation using weighted F1-score

### Result
- Validation Weighted F1-score: **84.33%**

---

## Exercise 2: Ticket Cancellation Prediction

**Objective:** Predict whether a ticket will be cancelled using the `Cancel` target variable.

### Dataset
- Training data: 101,017 records and 22 columns
- Test data: 43,293 records
- Target variable: `Cancel` (binary classification)
- Class distribution in the training data:
  - Not cancelled: 85,716
  - Cancelled: 15,301

### Workflow
- Removal of identifier and hashed columns
- Handling missing values in `VehicleType` and `VehicleClass`
- Feature engineering and extraction of date/time features
- Encoding categorical variables using `OrdinalEncoder`
- Conversion of Boolean features into numeric values
- Handling class imbalance using SMOTE
- Model training using `XGBClassifier`
- Model evaluation using weighted F1-score

### Result
- Validation Weighted F1-score: **97.76%**

---

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- XGBoost

## Key Learning Outcomes

- Data preprocessing and missing-value handling
- Feature engineering and categorical encoding
- Classification with tree-based ensemble models
- Handling imbalanced datasets
- Model evaluation using weighted F1-score

