# Diabetes Prediction using Machine Learning

## Dataset Overview

We are working with a dataset containing information related to diabetes, with 2000 rows and 9 columns. The feature columns include:

- **Pregnancies**: Number of times a woman has been pregnant.
- **Glucose**: Blood sugar level of a person.
- **BloodPressure**: Blood pressure level of a person.
- **SkinThickness**: Skin thickness of a person.
- **Insulin**: Insulin level of a person.
- **BMI**: Body mass index of a person.
- **DiabetesPedigreeFunction**: Diabetes pedigree function of a person.
- **Age**: Age of a person.
- **Outcome**: Outcome of a diabetes test (0 for no diabetes, 1 for diabetes).

## Domain Analysis

- **Pregnancies**: A risk factor for diabetes.
- **Glucose**: High levels indicate possible diabetes.
- **BloodPressure**: High levels are a risk factor for diabetes.
- **SkinThickness**: Indicates insulin resistance.
- **Insulin**: Low levels may indicate diabetes.
- **BMI**: High BMI increases the risk of diabetes.
- **DiabetesPedigreeFunction**: Measures genetic risk.
- **Age**: Risk increases with age.

## Exploratory Data Analysis

### Bivariate Analysis

- Identified outliers in the Pregnancy column.
- Corrupted values (0) in Glucose, Blood Pressure, Skin Thickness, Insulin, BMI.
  
### Visualizations

- Pregnancy count vs. Diabetes risk.
- Blood Pressure, Skin Thickness, Insulin, BMI vs. Diabetes risk.
- Scatterplot showing relationships between Insulin, Glucose, and Diabetes risk.
- Diabetes risk increases with age.

### Data Cleaning

- Dropped duplicated rows.
- Checked for null values (none found).
- Dealt with corrupted values by dropping or imputing median values.

### Outliers

- Identified and addressed outliers in feature columns.

## Model Evaluation

- No high correlation between columns.

### Accuracy Scores

- Logistic Regression: 74.49%
- KNeighbors Classifier: 71.81%
- Random Forest Classifier: 74.50%
- Decision Tree Classifier: 73.82%
- XGBoost Classifier: 71.14%

## Conclusion

The analysis provides insights into diabetes risk factors and uses machine learning models to predict diabetes with varying accuracies. Further optimization and feature engineering may improve model performance.

Feel free to explore the Jupyter notebook for a detailed walkthrough.
