Lungs Cancer Survival Analysis and Prediction
Author: Pramod Nagisetty
University: University of Leicester
Email: pn118@student.le.ac.uk

Project Overview
This project analyzes medical data to explore factors affecting patient survival and predicts survival outcomes using machine learning models. It includes comprehensive steps such as data exploration, visualization, feature engineering, data balancing, model training, evaluation, and reporting.

Dataset
The dataset is loaded from dataset_med.csv and includes medical features like age, BMI, cholesterol levels, cancer stage, smoking status, treatment types, and more. The target variable is survived (binary).

Key Steps
1. Data Loading and Overview
Loads the dataset and displays the first five records.

Provides basic metadata and statistical summaries of the features.

2. Exploratory Data Analysis (EDA)
Visualizes distributions of key features such as:

Survival outcome

Gender

Cancer stage

Smoking status

Age, BMI, and cholesterol

Includes a heatmap of feature correlations to understand interrelationships.

3. Label Encoding
Encodes categorical variables using LabelEncoder.

Converts family_history (Yes/No) to binary format.

Drops unnecessary columns like id, diagnosis_date, and end_treatment_date.

4. Correlation Analysis
Plots a heatmap of Pearson correlations to identify strongly related variables.

5. Feature-Based Survival Insights
Trends in survival rate over diagnosis years.

Boxplots of BMI and cholesterol by survival.

Survival heatmap based on cancer stage and treatment type.

Survival rate by top 10 countries with most patients.

Parallel coordinates plot showing how features differ by survival.

6. Data Balancing with SMOTE
Applies SMOTE to handle class imbalance in the target variable (survived).

Confirms balanced class distribution using Counter.

7. Data Splitting and Preprocessing
Splits the dataset into training, validation, and test sets (stratified).

Standardizes features using StandardScaler.

8. Model Training and Evaluation
Trains and evaluates the following models:

Logistic Regression

Random Forest

XGBoost (if installed)

Each model is assessed on:

Validation accuracy

Test accuracy

Confusion matrix

Classification report

The best-performing model is identified based on test accuracy.

Dependencies
This project requires the following Python libraries:

pandas

matplotlib

seaborn

scikit-learn

imbalanced-learn

numpy

(optional) xgboost

Install dependencies using:

bash
Copy
Edit
pip install pandas matplotlib seaborn scikit-learn imbalanced-learn numpy xgboost
Output
Descriptive statistics and visual EDA

Encoded and balanced dataset

Accuracy comparison of models (validation vs test)

Confusion matrix and detailed classification report for the best model

Survival insights across various medical and demographic features

Notes
SMOTE is used to prevent bias in the model due to class imbalance.

XGBoost is included optionally and runs only if installed.

All plots are clearly labeled and designed for interpretability.
