
# Travel Reason Prediction — MrBilit

## Overview
The goal of this exercise is to predict the reason for a user's trip based on MrBilit ticket data. The target variable, `TripReason`, distinguishes between the classes `Work` and `Int`.

## Dataset
- **Training set:** 101,017 rows and 22 columns
- **Test set:** 43,293 rows and 21 columns
- **Target variable:** `TripReason`
- **Classes:** `Work`, `Int`

## Workflow
1. **Exploratory Data Analysis (EDA):** Examined the dataset structure, data types, missing values, and target distribution.
2. **Data Cleaning:** Removed selected identifier and hash-related columns and handled missing values in `VehicleClass` and `VehicleType`.
3. **Feature Engineering:** Converted `Created` and `DepartureTime` into datetime features, including weekday, hour, and month.
4. **Categorical Encoding:** Used `OrdinalEncoder` with support for unseen categories.
5. **Data Splitting:** Split the training data into training and validation sets.
6. **Model Training:** Trained a `RandomForestClassifier` with 100 estimators.
7. **Prediction:** Generated predictions for the test set and prepared the submission DataFrame.

## Results
- **Model:** Random Forest Classifier
- **Validation weighted F1-score:** 84.33%

The classification report showed different precision and recall values for the `Work` and `Int` classes, indicating that model performance should be evaluated beyond a single aggregate metric.

## Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Notes
The validation score reflects performance on the selected validation split and does not guarantee the same performance on unseen data. Further improvements could include more systematic feature selection, alternative categorical encoding strategies, and hyperparameter tuning.
