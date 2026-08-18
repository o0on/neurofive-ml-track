# Housing Price Regression

## Overview

This project uses the Ames Housing dataset to predict house sale
prices using Linear Regression.

## Features

The selected features were:

- OverallQual
- OverallCond
- GrLivArea
- LotArea
- Neighborhood

Neighborhood was converted into numerical features using one-hot encoding.

## Model

A Linear Regression model from scikit-learn was trained using an
80/20 train-test split.

## Results

RMSE: 37404.53

R² Score: 0.8176

The R² score means that the model explains approximately 81.76% of
the variation in house prices based on the selected features.

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
