
# Classification

This folder contains four classification exercises covering different supervised learning algorithms, preprocessing techniques, class imbalance handling, model evaluation, and hyperparameter tuning.

## Exercises

### 01-NBA-Player-Career-Prediction

Predict whether an NBA player will continue playing in the league for the next five years.

* **Dataset:** 938 training samples, 402 test samples
* **Preprocessing:** Feature selection, train/validation split, standardization
* **Model:** Logistic Regression
* **Evaluation:** ROC-AUC
* **Reported Validation Score:** ~67.20%
* **Output:** Test predictions and submission file

**Topics:**

* Binary Classification
* Logistic Regression
* Train/Validation Split
* Standardization
* Class Distribution
* ROC-AUC
* Prediction & Submission

---

### 02-Pistachio-Classification

Classify pistachios into two varieties using numerical features extracted from pistachio images.

* **Classes:** `Kirmizi_Pistachio`, `Siit_Pistachio`
* **Dataset:** 1,718 training samples, 430 test samples
* **Features:** 16 image-derived numerical features
* **Preprocessing:** Label Encoding, Min-Max Scaling
* **Model:** K-Nearest Neighbors (KNN)
* **Hyperparameter Selection:** 5-Fold Cross-Validation
* **Best `k`:** 13
* **Evaluation:** Weighted F1-score
* **Validation Score:** ~87.81%
* **Output:** Test predictions and submission file

**Topics:**

* KNN
* Classification
* Min-Max Scaling
* Label Encoding
* Cross-Validation
* Hyperparameter Selection
* Weighted F1-score
* Image-Derived Features

---

### 03-Fraud-Detection

Classify financial transactions as fraudulent or legitimate.

* **Dataset:** 7,840 training samples, 2,614 test samples
* **Target:** `Class` (fraudulent / legitimate)
* **Preprocessing:** Standardization
* **Class Imbalance Handling:** SMOTE
* **Model:** Support Vector Classifier (SVC) with RBF Kernel
* **Evaluation:** Weighted F1-score
* **Validation Score:** ~99.87%
* **Output:** Test predictions and submission file

**Topics:**

* Binary Classification
* SVM / SVC
* RBF Kernel
* Standardization
* Class Imbalance
* SMOTE
* Weighted F1-score
* Classification Report
* Fraud Detection

> The `V1`–`V28` features were already obtained through dimensionality reduction before this exercise.

---

### 04-Income-Prediction

Predict whether an individual's annual income is above or below $50K using a Decision Tree classifier.

* **Dataset:** 25,000 training samples, 7,164 test samples
* **Target:** `income`
* **Preprocessing:** Missing-value handling, mode imputation, ordinal encoding, label encoding
* **Class Imbalance Handling:** SMOTE
* **Model:** Decision Tree
* **Hyperparameter Tuning:** GridSearchCV with 5-Fold Cross-Validation
* **Best Parameters:**

  * `criterion = entropy`
  * `max_depth = 10`
  * `min_samples_split = 10`
* **Best Cross-Validation Accuracy:** ~86.56%
* **Validation Weighted F1-score:** ~81.93%
* **Output:** Test predictions and submission file

**Topics:**

* Decision Tree
* Binary Classification
* Missing Value Handling
* Mode Imputation
* Ordinal Encoding
* Label Encoding
* Class Imbalance
* SMOTE
* Cross-Validation
* GridSearchCV
* Hyperparameter Tuning
* Weighted F1-score

---

## Main Topics

Across these exercises, the following classification concepts and techniques are practiced:

* Binary Classification
* Logistic Regression
* K-Nearest Neighbors (KNN)
* Support Vector Machines (SVM)
* Decision Trees
* Feature Scaling
* Standardization
* Min-Max Scaling
* Label Encoding
* Ordinal Encoding
* Missing Value Handling
* Train/Validation Split
* Cross-Validation
* Hyperparameter Tuning
* GridSearchCV
* Class Imbalance
* SMOTE
* ROC-AUC
* Weighted F1-score
* Classification Report
* Prediction & Submission

## Folder Structure

```text
03-Classification/
│
├── README.md
│
├── 01-NBA-Player-Career-Prediction/
│
├── 02-Pistachio-Classification/
│
├── 03-Fraud-Detection/
│
└── 04-Income-Prediction/
```
