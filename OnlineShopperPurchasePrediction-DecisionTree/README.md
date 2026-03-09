- Online Shopper Purchase Prediction using Decision Tree

- Project Overview
This project predicts whether an online website visitor will generate revenue (make a purchase) based on their browsing session data. The model is built using a Decision Tree Classifier and optimized using hyperparameter tuning.

- Dataset
The dataset used is **online_shoppers.csv**, which contains information about online visitor sessions including:

- Administrative pages visited
- Informational pages visited
- Product related pages
- Bounce rates
- Exit rates
- Page values
- Traffic type
- Visitor type
- Month and other session features

Target Variable:
- **Revenue** (1 = Purchase, 0 = No Purchase)

Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

Machine Learning Workflow

1. Data Loading
The dataset is loaded using pandas.

2. Data Preprocessing
Two types of preprocessing are applied:

- **StandardScaler** for numerical features
- **OneHotEncoder** for categorical features

This is implemented using **ColumnTransformer**.

### 3. Model
A **Decision Tree Classifier** is used to predict the revenue outcome.

### 4. Pipeline
A Scikit-learn **Pipeline** is created to combine preprocessing and the model.

### 5. Model Evaluation
Model performance is evaluated using:

- F1 Score
- Classification Report
- Confusion Matrix

### 6. Hyperparameter Tuning
GridSearchCV is used to find the best parameters for the Decision Tree model.

Parameters tuned:
- `max_depth`
- `min_samples_leaf`

## Results
The model performance is evaluated using the **F1 score**, which balances precision and recall and is suitable for imbalanced classification problems.
