# Exploring the Impact of Lifestyle and Health Factors on Diabetes Risk

This project investigates how modifiable lifestyle and health factors—such as **Body Mass Index (BMI)**, **physical activity**, and **blood pressure** contribute to the risk of developing Type 2 diabetes. Using the **Behavioral Risk Factor Surveillance System (BRFSS)** dataset and a combination of **statistical analysis** and **machine learning models**, we aim to uncover insights and build predictive models for early diabetes risk detection.

## Dataset

- **Source**: [CDC BRFSS (Behavioral Risk Factor Surveillance System)](https://www.cdc.gov/brfss/)
- **Format**: CSV
- **Attributes**: Diabetes status, BMI, blood pressure, cholesterol, smoking, physical activity, diet, general health, demographics, etc.

## Methods Used

- **Statistical Analysis**:  
  - Chi-Square Test (association between categorical variables)  
  - T-Test (comparison of BMI between diabetic and non-diabetic groups)

- **Machine Learning Models**:  
  - Random Forest  
  - XGBoost  
  - Resampling techniques (e.g., ROSE) for class imbalance

- **Programming Language**: R

## Objectives

- Identify significant predictors of diabetes.
- Evaluate the association between lifestyle choices and diabetes prevalence.
- Build and evaluate predictive models for diabetes risk classification.

## Key Findings

- Higher **BMI**, **lack of physical activity**, and **high blood pressure** are strongly associated with diabetes.
- **XGBoost** outperformed other models in predictive accuracy and feature importance.
- Resampling improved model balance for minority classes (diabetic individuals).

## Files in this Repository

| File Name                            | Description |
|-------------------------------------|-------------|
| `diabetes_dataset.csv`              | Cleaned dataset used for analysis |
| `VariableTable.xlsx`                | Metadata explaining each variable |
| `Diabetics_analysis.Rmd`            | R Markdown notebook containing the full analysis |
| `Diabetics_analysis.nb.html`        | Rendered HTML of the R notebook |
| `Diabetics_analysis.docx`           | Report format of the analysis |

## Visualizations

- Distribution plots for BMI, physical activity, and blood pressure
- Bar plots showing diabetes prevalence by category
- Feature importance plots from machine learning models

## How to Run

1. Clone the repository.
2. Open the `.Rmd` file in RStudio or run the `.html` file in a browser to view the output.
3. Ensure the following R packages are installed:
   ```r
   tidyverse, openxlsx, dplyr, MASS, pscl, pROC, car, ggplot2, corrplot
