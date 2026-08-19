# Titanic Survival Classification

## Overview

This project uses the Titanic dataset to predict whether a passenger
survived using Logistic Regression.

## Approach

- Cleaned missing values
- Encoded categorical features
- Split the dataset into training and testing sets
- Trained a Logistic Regression model
- Evaluated using accuracy and a confusion matrix

## Results

Final Accuracy: 81.01%

## Hyperparameter Tuning

GridSearchCV was used to tune two Logistic Regression hyperparameters:
`C` and `solver`. Five values of `C` and two different solvers were
tested using 5-fold cross-validation.

The best parameters were `C=1` and `solver='liblinear'`, with a
cross-validation accuracy of approximately 79.63%.

### Before vs After

| Metric | Original | Tuned |
|---|---:|---:|
| Accuracy | 81% | 79% |
| Precision | 79% | 77% |
| Recall | 74% | 72% |
| F1-score | 76% | 74% |

The tuned model performed slightly worse on the test set than the
original model. This demonstrates that hyperparameter tuning does not
always improve performance on unseen data. In this case, the original
Logistic Regression model generalized slightly better to the test set.

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
