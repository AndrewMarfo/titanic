# Titanic

This project focuses on the analysis of the Titanic dataset, incorporating both exploratory data analysis (EDA) and machine learning models to predict survival outcomes. The analysis uncovers patterns, relationships, and key insights related to passenger survival, demographics, and other relevant features.

## Project Overview

The Titanic dataset provides information about passengers aboard the Titanic, including their survival status, age, sex, class, and other attributes. This analysis aims to:

- Perform data cleaning and preprocessing to handle missing or inconsistent data.
- Conduct EDA to understand key patterns and relationships within the dataset.
- Implement and evaluate machine learning models to predict survival.
- Generate visualizations to communicate insights effectively.

There are three datasets:
- `train.csv`: contains the training data with 712 rows and 12 columns.
- `test.csv`: contains the test data with 179 rows and 11 columns.
- `Andrew_submission.csv`: contains the submission data (Predicted data) with 179 rows and 1 column.


## Features

Key features of the dataset include:

- **Survived**: Survival status (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Sex**: Gender of the passenger
- **Age**: Age of the passenger
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Fare**: Passenger fare
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Process

### 1. Data Loading and Exploration
- Loaded the Titanic dataset.
- Inspected the dataset structure using functions like `head()`, `info()`, and `describe()`.

### 2. Data Cleaning
- Imputed missing values in columns such as `Age`, `Cabin` and `Embarked`.
- Dropped unnecessary columns and converted data types as needed.

### 3. Feature Engineering
- Encoded categorical variables using `LabelEncoder`.
- Normalized numerical features to ensure uniform scaling.

### 4. Exploratory Data Analysis (EDA)
- Performed univariate, bivariate, and multivariate analyses.
- Visualized relationships between survival and other features (e.g., `Pclass`, `Sex`, `Age`).

### 5. Machine Learning Models

#### Implemented Models:
- Logistic Regression
- Random Forest Classifier
- K-Nearest Neighbors (KNN)

#### Steps:
- Split data into training and validation sets using `train_test_split`.
- Trained models and evaluated performance using metrics like accuracy, precision, recall, and F1-score.
- Performed hyperparameter tuning using `GridSearchCV` for optimal model performance.

#### Results:
- The best-performing model was the Random Forest Classifier with an accuracy of 85% and precision of 84%.

#### Prediction:
- Used the chosen model to predict survival on the test dataset.

## Tools and Libraries

This analysis was conducted using:

- **Python**
- **Jupyter Notebook**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Scikit-learn**: Machine learning and evaluation
- **Matplotlib & Seaborn**: Data visualization

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/AndrewMarfo/titanic.git
   ```

2. Navigate to the project directory and open the Jupyter Notebook:
   ```bash
   cd titanic
   jupyter notebook
   ```

3. Run the cells sequentially to execute the analysis.

## Key Insights

- Gender and class significantly influence survival rates.
- Younger passengers had a higher likelihood of survival.
- First-class passengers had the highest survival rates.
- Random Forest Classifier was the best model for predicting survival.
