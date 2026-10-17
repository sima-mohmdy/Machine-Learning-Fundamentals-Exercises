
# Fake News Detection

## Overview
This project focuses on classifying news articles as **Fake** or **Real** using a Support Vector Machine (SVM). The dataset includes preprocessed text vectors and metadata such as author, publication date, website, and news type.

## Dataset
The dataset is divided into training and test sets.

| File | Shape | Description |
|---|---:|---|
| `news_train.csv` | 1500 × 5 | Training metadata and labels |
| `news_test.csv` | 346 × 4 | Test metadata |
| `news_train_text_vectors.npz` | 1500 × 42141 | Training text vectors |
| `news_test_text_vectors.npz` | 346 × 42141 | Test text vectors |

The target variable is `label`, with two classes: `Fake` and `Real`.

## Methods
- **Exploratory Data Analysis:** Examining dataset dimensions, missing values, and target distribution.
- **Feature Engineering:** Extracting year, month, hour, day of the week, and weekend indicators from publication dates.
- **Preprocessing:** Encoding categorical features, scaling numerical features, and handling missing values.
- **Dimensionality Reduction:** Applying Truncated SVD to reduce text features to 300 components.
- **Model Training:** Training an SVM classifier with a linear kernel and class weighting.
- **Model Evaluation:** Using F1-score, classification reports, and confusion matrices.
- **Model Comparison:** Investigating the effects of feature selection, class weights, the `C` parameter, and kernel choice.

## Experiments and Results

### 1. Initial Model
The initial model achieved an F1-score of **1.00** on the validation set. Further investigation showed that the `type` feature was perfectly associated with the target labels in this dataset split, making it an unreliable shortcut for evaluating genuine news-content classification.

### 2. Removing the `type` Feature
After excluding `type`, the model achieved:
- Binary F1-score (Real class): **0.8487**
- Weighted F1-score: **0.9021**

### 3. Removing Both `type` and `author`
Using only temporal and text features reduced performance:
- Binary F1-score (Real class): **0.6768**
- Weighted F1-score: **0.7747**

### 4. Model Selection
Experiments with the original text vectors showed that:
- A linear kernel outperformed the RBF kernel.
- `C = 1.0` performed better than the other tested values.
- Class weighting improved the F1-score for the Real class.
- Using text features alone produced a weighted F1-score of **0.7817**.

### Final Model
The final model uses a linear SVM with `C = 1.0` and `class_weight='balanced'`, trained on the original text vectors without dimensionality reduction or metadata features.

| Metric | Validation Score |
|---|---:|
| Accuracy | 0.7893 |
| F1-score (Real class) | 0.6520 |
| Weighted F1-score | 0.7817 |

## Test Predictions
The final model predicts labels for all 346 test samples. Predictions are saved in `submission.csv`, containing a single column named `label`.

## Technologies
- Python
- NumPy
- Pandas
- SciPy
- Scikit-learn
- Google Colab

## Key Takeaways
- Text classification can be approached using classical machine learning when text is provided as numerical feature vectors.
- Dimensionality reduction can reduce computational cost, but may also discard useful information.
- A perfect validation score can be misleading when a feature acts as a shortcut for the target.
- Evaluating different feature sets and model configurations provides a more informative picture of model performance.
