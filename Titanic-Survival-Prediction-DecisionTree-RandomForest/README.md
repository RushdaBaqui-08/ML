# Titanic Survival Prediction using Decision Tree and Random Forest

This project predicts whether a passenger survived the Titanic disaster using Machine Learning models.

The project demonstrates the use of **Decision Tree** and **Random Forest** classifiers and compares their performance.

## Dataset
The dataset is loaded using the **Seaborn Titanic dataset**.

Features used:
- pclass (Passenger class)
- sex
- fare
- embarked
- age

Target variable:
- survived

## Steps Performed

1. Data Loading
   - Titanic dataset loaded using seaborn

2. Data Preprocessing
   - Missing values handled using `SimpleImputer`
   - Median strategy used for age
   - Most frequent strategy used for embarked
   - Categorical variables encoded using `LabelEncoder`

3. Train Test Split
   - Dataset split into training and testing sets

4. Decision Tree Model
   - Trained using `DecisionTreeClassifier`
   - Tree visualization using `plot_tree`
   - Training and testing accuracy calculated

5. Random Forest Model
   - Trained using `RandomForestClassifier`
   - Used 501 trees
   - Out-of-Bag (OOB) score calculated
   - Testing accuracy evaluated

## Libraries Used

- pandas
- seaborn
- matplotlib
- scikit-learn

## Results

The Decision Tree model shows signs of **overfitting**, while the Random Forest model provides **better generalization and performance**.
