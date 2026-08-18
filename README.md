# TitanSic Survival Prediction

## Project Overview

This project uses the Titanic dataset from Kaggle to build a machine learning
classification model that predicts whether a passenger survived or did not survive.

## Data Preparation

The dataset was first explored using pandas to understand its structure and
identify missing values. Missing values in the Age column were replaced with
the median age, while missing Embarked values were replaced with the most
frequent value. The Cabin column was removed because a large portion of its
values were missing.

## Features

The following features were used to predict survival:

- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked

The categorical features Sex and Embarked were converted into numerical
features using one-hot encoding with pandas `get_dummies()`.

## Machine Learning Model

A Logistic Regression model from scikit-learn was used for classification.
The dataset was divided into 80% training data and 20% testing data using
`train_test_split()`.

## Evaluation

The model was evaluated using accuracy and a confusion matrix.

Final Accuracy:

**81.01%**

The confusion matrix was used to identify correct and incorrect predictions,
including passengers who were correctly or incorrectly predicted as survivors
or non-survivors.

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Conclusion

The Logistic Regression model was able to predict passenger survival with an
accuracy of 81.01%. This project demonstrated the basic machine learning
workflow of data preparation, feature encoding, train/test splitting, model
training, prediction, and evaluation.
