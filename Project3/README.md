# Predictive Modeling for Loan Default Risk Assessment

## Project Overview
This project aims to build a machine learning model that predicts the likelihood of a borrower defaulting on a loan. By accurately predicting loan defaults, banks can make better lending decisions, reducing their exposure to bad debts and improving financial stability.

## Data Description
The dataset used for this project is the **Loan Default Dataset**. Due to its large size, the original dataset was split into two CSV files: `Loan_Default1.csv` and `Loan_Default2.csv`. These two files are merged during the data preprocessing stage in our code.

### Files Included
- `EDA.Rmd`: R Markdown file containing the Exploratory Data Analysis (EDA).
- `Final_Report (Team069).pdf`: The final report of the project detailing the methodology, analysis, and findings.
- `Loan_Default1.csv`: The first part of the loan default dataset.
- `Loan_Default2.csv`: The second part of the loan default dataset.
- `README.md`: This file, providing an overview of the project.
- `model_pipeline_final.Rmd`: R Markdown file detailing the final model pipeline and analysis.

## Objective
The primary objective of this project is to construct and refine a model that can accurately predict the likelihood of loan defaults based on various borrower and loan characteristics.

## Methodology
### Data Cleaning and Preprocessing
- **Merging Datasets**: The two CSV files, `Loan_Default1.csv` and `Loan_Default2.csv`, are merged to create a single dataset.
- **Handling Missing Values**: Missing values were managed using advanced imputation techniques, particularly with bagged models.
- **Feature Selection**: Non-informative features were removed to improve model performance.
- **Data Transformation**: Categorical variables were converted into dummy variables, and the target variable was transformed into a binary categorical variable for logistic regression.

### Models Used
- **Random Forest**: Selected as the best model due to its superior performance in accuracy and ROC AUC.
- **LightGBM**: Implemented for its computational efficiency but was outperformed by the Random Forest model.
- **Logistic Regression**: Used as a baseline model.

## Results
The Random Forest model was found to be the most reliable for predicting loan defaults. It outperformed other models in both accuracy and ROC AUC, making it the preferred model for deployment.

## Final Model and Key Predictors
The final Random Forest model identified the following as the most important predictors of loan defaults:
1. **Credit Type**
2. **Loan-to-Value Ratio (LTV)**
3. **Income**
4. **Debt-to-Income Ratio (DTIR)**
5. **Property Value**
6. **Credit Score**
7. **Loan Amount**

## Conclusion
This project demonstrates the application of advanced machine learning techniques in predicting loan defaults. The resulting model provides banks with a powerful tool for risk assessment, leveraging critical borrower information to make more informed lending decisions.

## How to Run the Project
1. **Clone the repository**: Clone this repository to your local machine.
2. **Install necessary packages**: Ensure you have all required R packages installed.
3. **Run the analysis**: Execute the `.Rmd` files in the order provided (`EDA.Rmd` first, followed by `model_pipeline_final.Rmd`) to reproduce the analysis and results.


