
# Mall Customer Segmentation

##  Overview
In this exercise, customer segmentation is performed on a mall customer dataset using **K-Means clustering**. The goal is to identify groups of customers with similar characteristics to support customer analysis and targeted marketing strategies.

## Dataset
The dataset contains 200 customers and the following features:

- `CustomerID`: Unique customer identifier
- `Gender`: Customer gender
- `Age`: Customer age
- `Annual Income (k$)`: Annual income in thousands of dollars
- `Spending Score (1-100)`: Customer spending score

There is no target variable because this is an **unsupervised learning** task.

##  Preprocessing and Feature Engineering
A custom `Preprocessor` class is implemented to prepare the data for clustering.

The preprocessing steps include:

- Applying a logarithmic transformation to annual income
- Removing `CustomerID`, `Gender`, and the original income column
- Handling missing values
- Standardizing the resulting numerical features using `StandardScaler`

The preprocessing pipeline is saved in `preprocessor.py` for use during evaluation.

##  Model
The **K-Means** algorithm from Scikit-learn is used to cluster customers.

The number of clusters is evaluated using the **Silhouette Score**, which measures how well-separated and compact the resulting clusters are.

##  Evaluation
The model is evaluated using the Silhouette Score. The Quera score is calculated as:

\[
\text{Score} = 100 \times \frac{\text{Silhouette Score} + 1}{2}
\]

The reported Silhouette Score for the six-cluster configuration is approximately **0.4486**, corresponding to a Quera score of approximately **72.43**.

##  Files
- `mall_customer_segmentation_3.ipynb`: Notebook containing data exploration, preprocessing, clustering, and evaluation
- `preprocessor.py`: Custom preprocessing class
- `submission.csv`: Predicted cluster assignments for all 200 customers
- `model`: Saved K-Means model

##  Technologies
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib / Seaborn

##  Key Concepts
- Unsupervised Learning
- Customer Segmentation
- K-Means Clustering
- Feature Engineering
- Log Transformation
- Feature Scaling
- Silhouette Score
- Hyperparameter Tuning
