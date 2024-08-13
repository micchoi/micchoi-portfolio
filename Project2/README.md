# ClarityAI Final Project: CO2 Emissions Prediction

## Overview

This repository contains the code and final report for the ClarityAI CO2 Emissions Prediction project. The objective of this project was to develop predictive models for CO2 emissions using historical data from various companies worldwide. The project focuses on assessing the effectiveness of different environmental commitments, such as emission targets and policies, and their impact on CO2 emissions.

## Repository Structure

- **ClarityAI_FinalReport (Team 4).pdf**: The final report summarizing the entire project, including data analysis, modeling, results, and conclusions.

- **EDA.ipynb**: The Jupyter Notebook containing the Exploratory Data Analysis (EDA). This notebook explores the dataset, visualizes trends, and identifies key patterns and relationships.

- **Modeling (log transformation).ipynb**: The Jupyter Notebook that details the modeling process. It includes data preprocessing, feature engineering, model training, and evaluation. The notebook uses log transformation for some features to address skewness.

- **requirements_eda.txt**: A text file listing the Python libraries and dependencies required to run the EDA notebook.

- **requirements_modeling.txt**: A text file listing the Python libraries and dependencies required to run the modeling notebook.

## Data Description

The dataset used in this project is panel data consisting of company-level information from 2002 to 2022. Each company is represented across these years with various features such as CO2 emissions, revenue, and specific environmental commitments. The data is organized by:
- **Country**: The country where each company's headquarters is located.
- **Industry**: The industry classification of each company.
- **Company**: Individual companies tracked across the years.

**Note**: The dataset used in this project is not included in this repository due to contractual agreements with ClarityAI. Access to the data is restricted, and those interested in the dataset should contact ClarityAI directly.

## Getting Started

To run the EDA or Modeling notebooks, follow these steps:

1. **Clone the Repository**: 
   ```bash
   git clone https://github.com/micchoi/micchoi-portfolio.git
2. **Install Dependencies**
   pip install -r requirements_eda.txt
   pip install -r requirements_modeling.txt
4. **Run the Notebooks**
   Open the EDA or Modeling notebooks using Jupyter Notebook or Jupyter Lab and run the cells sequentially.
