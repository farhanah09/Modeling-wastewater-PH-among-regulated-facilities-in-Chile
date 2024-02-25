# Overview

This project investigates factors contributing to deviations in wastewater pH levels among regulated facilities in Chile. Utilizing a dataset containing pH measurements, reporting compliance metrics, and facility information, the goal is to:

- Identify key predictors of pH deviations from neutrality.
- Build predictive models to estimate the likelihood of significant pH deviations.
- Potentially inform strategies to improve environmental compliance.

## Methods

### Data Preprocessing:

Cleaning and filtering of the 'chilePHdata.csv' dataset.
Calculation of absolute pH deviation from 7 as the target variable.

### Exploratory Analysis:

Visualization of pH deviation distributions.

### Regression Modeling:

Implementation of Ridge, Lasso, and Elastic Net regression models.
Use of cross-validation (cv.glmnet) for hyperparameter tuning (lambda and alpha).
Comparison of model performance and variable importance.

### Evaluation:

Splitting the dataset into training (80%) and testing (20%) sets.
Evaluation of model performance on the held-out test set using appropriate metrics.
Key Findings (Replace with your actual results)

Example: Lasso regression identified measurement type, reporting frequency, and the number of previous infractions as the most significant predictors of pH deviation.
Example: Elastic Net with an alpha of 0.5 demonstrated superior performance on the test set, achieving a mean squared error of X.

## Repository Structure

chilePHdata.csv: Original dataset.
wastewaster_model.rmd
README.md: This file.

## Dependencies

R (version X.X.X)
tidyverse
glmnet
caret
