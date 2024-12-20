# Loan_Prediction
Loan Eligibility Prediction
This project involves predicting loan eligibility for customers applying for home loans. Dream Housing Finance Company aims to automate the loan eligibility process based on customer information. This README provides an overview of the project, its structure, and instructions for running the solution.

### Problem Statement
Dream Housing Finance Company deals in all kinds of home loans and operates across urban, semi-urban, and rural areas. The company wants to     automate the loan eligibility process (in real-time) based on customer details provided in online application forms. These details include       Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History, and others.
The objective is to predict loan eligibility (Yes/No) for customers.

### Dataset
    The dataset consists of two files:
        1. Train.csv: Contains customer details and the target variable Loan_Status (Yes/No).
        2. Test.csv: Contains similar data without the target variable, used for evaluation.
Key Features:
- Loan_ID: Unique Loan ID
- Gender: Male/Female
- Married: Applicant married (Y/N)
- Dependents: Number of dependents
- Education: Graduate/Undergraduate
- Self_Employed: Self-employed (Y/N)
- ApplicantIncome: Applicant's income
- CoapplicantIncome: Co-applicant's income
- LoanAmount: Loan amount in thousands
- Loan_Amount_Term: Term of loan in months
- Credit_History: Credit history meets guidelines (1: Yes, 0: No)
- Property_Area: Urban/Semi-Urban/Rural
- Loan_Status: (Target) Loan approved (Y/N)

### Solution Workflow
   ### 1. Data Preprocessing
        Handling Missing Values: Imputation for missing values in LoanAmount, Gender, and other features.
        Feature Engineering: Created new features, such as total income (ApplicantIncome + CoapplicantIncome).
        Categorical Encoding: Used Label Encoding for binary variables and One-Hot Encoding for multi-category variables.
   ### 2. Exploratory Data Analysis (EDA)
        Analyzed distributions of numerical features and relationships between predictors and the target variable.
        Identified key patterns and trends in loan approval rates based on income, credit history, and property area.
   ### 3. Model Development
        Splitted the data into training and validation sets.
        Used classification models, including:
            Logistic Regression
            Decision Trees
            Random Forest
            Gradient Boosting (e.g., XGBoost, LightGBM)
        Performed hyperparameter tuning using GridSearchCV/RandomizedSearchCV.
   ### 4. Evaluation Metrics
        Used Accuracy to evaluate model performance.
        Compared performance across different models and selected the best-performing one.
