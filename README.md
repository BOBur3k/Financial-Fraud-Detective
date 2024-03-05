# Financial-Fraud-Detective
![Dalle2_ART](docs/imagee.jpg)
<p align="right">
  Artwork created by AI
</p>

## Project Overview

This project aims to build a machine learning pipeline to detect fraudulent transactions in a synthetic dataset of bank transactions. The pipeline includes steps such as exploratory data analysis (EDA), data cleaning, model creation, hyperparameter tuning, and model evaluation.

## Background

Financial fraud detection involves identifying fraudulent transactions within a dataset that predominantly consists of legitimate transactions. This project addresses the challenge of imbalanced datasets, where fraudulent transactions are the minority class. The goal is to create a model that effectively captures fraudulent transactions while minimizing false positives.

## Project Structure

The project follows a structured approach with the following notebooks:

1. **Initial EDA**:
   - Conduct univariate, bivariate, and multivariate exploratory analysis.
   - Formulate hypotheses based on insights gained from the analysis.
   - Explore relationships between predictors and the target variable.
   
2. **Data Cleaning and Pre-processing**:
   - Clean and wrangle the dataset.
   - Handle missing values, outliers, and incorrectly formatted data.
   - Drop unnecessary columns based on EDA findings.
   - Save the pre-processed dataset for further analysis.

3. **Model Creation and Evaluation**:
   - Split the pre-processed dataset into training and testing sets.
   - Implement a RandomForestClassifier or GradientBoostingClassifier.
   - Perform hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
   - Evaluate the model's performance using metrics such as accuracy and F1 score.

4. **Report**:
   - Answer specific questions related to the project in a separate document.
   - Summarize insights gained from EDA.
   - Explain the criteria for selecting columns to drop or keep.
   - Describe the hyperparameter tuning strategy used and its impact on model performance.
   - Present the final F1 score achieved by the model.

## Progress Summary

### EDA Highlights:
- Explored a dataset with over 600,000 transactions.
- No missing values identified.
- Diverse data types: float64, int64, and object.
- Discovered that 'isFlaggedFraud' column is indicative of poor fraud detection compared to actual fraud transactions.
- Found that most frauds occur in CASH_OUT and TRANSFER transactions.

### Model Evaluation Results:
- Achieved 100% accuracy on the training set and 99.96% accuracy on the test set with a RandomForestClassifier.
- Observed a discrepancy in recall between fraudulent and non-fraudulent transactions in the test set.
