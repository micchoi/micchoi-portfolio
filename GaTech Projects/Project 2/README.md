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

## Dependencies

To ensure that others can reproduce the results of this analysis, we use `renv` for package management. Follow the steps below to set up your environment:

1. **Clone the Repository**:
    Cloning the repository creates a local copy of the project on your machine, including all files and the directory structure. This ensures you have the exact same setup for reproducibility:
    ```sh
    git clone https://github.com/micchoi/micchoi-portfolio.git
    cd micchoi-portfolio/Project1  # Navigate to the desired project directory
    ```

2. **Restore the `renv` Environment**:
    Use `renv` to restore the project environment to the state captured in the `renv.lock` file. This ensures that all necessary packages and their correct versions are installed:
    ```r
    library(renv)
    renv::restore()
    ```

    This command will install the required package versions to match the environment used for this analysis.

3. **Run the R Markdown Files**:
    After restoring the environment, open the `.Rmd` files (e.g., `EDA.Rmd` and `model_pipeline_final.Rmd`) in your preferred R IDE (such as RStudio) and run them to reproduce the analysis. Make sure to run them in the order specified in the workflow section.

    Alternatively, you can knit the `.Rmd` files directly to generate the output documents:
    ```r
    rmarkdown::render("EDA.Rmd")
    rmarkdown::render("model_pipeline_final.Rmd")
    ```

By following these steps, you will set up the same environment used in the project, ensuring consistent and reproducible results.


