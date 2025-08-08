# Diabetes Prediction using Decision Tree Classifier

## Project Overview
Diabetes is a chronic disease characterized by high blood sugar levels. It can lead to severe health complications, including heart disease, kidney failure, and nerve damage.  
According to Sisodia and Sisodia (2018), diabetes is one of the most deadly and persistent conditions worldwide. There are two main types:  
- **Type I:** Common in individuals under 30, caused by the pancreas failing to produce insulin.  
- **Type II:** More common in older individuals, caused by insulin resistance.

This project applies a **Decision Tree Classifier** to predict diabetes based on several health measurements.

## Objective
To build a classification model that predicts whether a patient has diabetes using health-related features.

## Dataset
- **Rows:** 768  
- **Columns:** 9  
  - Pregnancies  
  - Glucose  
  - Blood Pressure  
  - Skin Thickness  
  - Insulin  
  - BMI  
  - Diabetes Pedigree Function  
  - Age  
  - Outcome (1 = diabetic, 0 = non-diabetic)  
- **Missing Values:** None after imputation  

## Methodology

### 1. Data Preprocessing
- Checked for missing values  
- Identified placeholder zeros in some medical measurements  
- Imputed missing/placeholder values with median  

### 2. Exploratory Data Analysis (EDA)
- Created correlation heatmap for all variables  
- Visualized distributions of Age and BMI using histograms  

### 3. Model Implementation
- Split data into features (X) and target (y)  
- Train-test split: 80% training, 20% testing  
- Model: `DecisionTreeClassifier` (max_depth=3)  
- Evaluated model using accuracy score, confusion matrix, classification report, ROC curve & AUC  

## Results & Insights
- Highest correlations:  
  - BMI & Skin Thickness: 0.54  
  - Age & Pregnancies: 0.54  
  - Glucose & Outcome: 0.49  
- Accuracy: 72.1%  
- Precision: Diabetic = 0.603, Non-diabetic = 0.603  
- Recall: Diabetic = 0.768, Non-diabetic = 0.636  
- F1-score: Diabetic = 0.779, Non-diabetic = 0.619  
- Confusion Matrix:  
  - True Negative (TN) = 76  
  - True Positive (TP) = 35  
  - False Negative (FN) = 20  
  - False Positive (FP) = 23  
- AUC: 0.70  

##  Technologies Used
- Python  
- Libraries: `NumPy`, `Pandas`, `Matplotlib`, `Seaborn`, `scikit-learn`, `os`



