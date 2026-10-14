
# Ensemble Learning

This folder contains machine learning exercises focused on ensemble learning algorithms for classification tasks. The exercises cover data preprocessing, model training, evaluation, class imbalance handling, and hyperparameter tuning.

## Exercises

### 1. Mushroom Hunter

**Objective:**  
Classify mushrooms as edible or poisonous based on their physical characteristics.

**Dataset:**
- Training set: 6,499 samples
- Test set: 1,625 samples
- Features: 22 categorical features
- Target variable: `class` (`e` = edible, `p` = poisonous)

**Workflow:**
- Exploratory Data Analysis (EDA)
- Missing value identification and imputation
- Categorical feature encoding using `LabelEncoder`
- Train/validation split
- Model training using `RandomForestClassifier`
- Evaluation using macro Recall
- Test-set prediction and submission generation

**Validation Result:**
- Macro Recall: **100%**

**Key Concepts:**
- Random Forest Classification
- Categorical Data Preprocessing
- Missing Value Handling
- Label Encoding
- Model Evaluation

### 2. Bank Customers

**Objective:**  
Predict whether a customer will subscribe to a term deposit based on historical bank marketing campaign data.

**Dataset:**
- Training set: 39,188 samples
- Test set: 2,000 samples
- Features: Customer demographics, campaign information, previous contact outcomes, and economic indicators
- Target variable: `y` (`yes` or `no`)

**Workflow:**
- Exploratory Data Analysis (EDA)
- Missing value analysis and imputation
- Stratified train/validation split
- Categorical feature encoding using One-Hot Encoding
- Feature alignment across training, validation, and test sets
- Class imbalance handling using `SMOTE`
- Model training using `AdaBoostClassifier`
- Evaluation using macro F1-score
- Hyperparameter tuning using `GridSearchCV`
- Test-set prediction and submission generation

**Model Configuration:**
- Algorithm: AdaBoost Classifier
- `n_estimators`: 100
- `learning_rate`: 1.0
- `random_state`: 0

**Validation Results:**
- Macro F1-score: **76.48%**

**Hyperparameter Tuning:**
- Method: `GridSearchCV`
- Cross-validation: 5-fold
- Scoring metric: Macro F1-score
- Best parameters: `n_estimators = 100`, `learning_rate = 1.0`
- Best cross-validation score: **92.02%**

**Key Concepts:**
- AdaBoost Classification
- Ensemble Learning and Boosting
- Missing Value Imputation
- One-Hot Encoding
- Class Imbalance and SMOTE
- Macro F1-score
- Cross-Validation
- Hyperparameter Tuning

## Skills Practiced

- Ensemble Learning: Random Forest and AdaBoost
- Data Cleaning and Preprocessing
- Categorical Feature Encoding
- Imbalanced Classification
- Model Training and Evaluation
- Cross-Validation and Hyperparameter Tuning
- Test-Set Prediction and Submission Preparation
