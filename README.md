# Titanic-Survival-Prediction---Classification-Task
This project applies Machine Learning classification models to predict the survival of passengers aboard the Titanic. The models implemented are:  Logistic Regression  Random Forest (with hyperparameter tuning)  The project involves data preprocessing, feature engineering, visualization, model training, cross-validation, and evaluation.  

**📊 Dataset**

The dataset is derived from the Kaggle Titanic Survival dataset.

**Features:**

**survival:** Survival (0 = No, 1 = Yes)

**pclass:** Passenger class (1st = Upper, 2nd = Middle, 3rd = Lower)

**sex:** Gender of passenger

**age:** Age in years (fractional if < 1, xx.5 if estimated)

**sibsp:** Number of siblings/spouses aboard

**parch:** Number of parents/children aboard

**ticket:** Ticket number

**fare:** Passenger fare

**cabin:** Cabin number

**embarked:** Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

**titanic survival data dictionary**

**⚙️ Methodology**

**Data Preprocessing**

Removal of Cabin (too many missing values)

Imputation: median age by sex & class, most frequent embarkation, mean fare for missing entries

Feature engineering: Title extracted from Name, Family_size derived from sibsp + parch + 1

Encoding categorical variables using OneHotEncoder

Scaling age and fare with MinMaxScaler

**Visualization**

Count plots for gender-based survival

Correlation heatmaps

Pair plots for feature interactions

**Models Implemented**

Logistic Regression

Random Forest (GridSearchCV hyperparameter tuning: n_estimators, max_depth, min_samples_split, min_samples_leaf)

**Evaluation**

Cross-validation (5-fold)

Logistic Regression: 0.8260

Random Forest: 0.8092

Validation accuracy: 0.8380 (Random Forest)

**🚀 Results & Insights**

Logistic Regression performed slightly better in cross-validation.

Random Forest, after tuning, showed higher validation performance on unseen data.

Gender (sex), passenger class (pclass), and fare were strong predictors of survival.

Feature engineering (Title, Family_size) improved prediction quality.

**📖 Files**

Jupyter Notebook (HTML)
 → Implementation and visualizations.

Data Dictionary
 → Explanation of dataset features.

**🛠️ Requirements**

If you want to re-run this project in Python, you will need:

python >= 3.8
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter

**📌 Usage**

Open the Jupyter Notebook (not included here but HTML provided).

jupyter notebook

Explore the report for methodology and findings.

**📜 License**

This project is for academic purposes. Free to use and adapt with attribution.
