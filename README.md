# Building Insurance Claim Prediction

This repository contains a project to build a binary classification model that predicts the probability of having at least one insurance claim over the insured period of a building. The prediction is based on the building's characteristics. The model is developed using Python and includes ROC curves and AUC values for both training and testing datasets.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Results](#results)

## Introduction
This project aims to predict whether a building will have an insurance claim during a certain period based on its characteristics. The target variable `Claim` is a binary variable where 1 indicates that there is at least one claim, and 0 indicates no claims.

## Dataset
The dataset used for this project is `data.csv`. It contains various features related to buildings and a target variable `Claim`.

## Preprocessing
The data preprocessing steps include:
1. Handling missing values using `SimpleImputer`.
2. Encoding categorical variables using `OneHotEncoder`.
3. Standardizing numeric features using `StandardScaler`.

## Modeling
The model is built using Logistic Regression. A pipeline is used to streamline the preprocessing and modeling steps. 

## Evaluation
The model's performance is evaluated using ROC curves and AUC scores for both the training and testing datasets. These metrics help assess the model's ability to distinguish between classes.

## Results
- **Training ROC AUC:** The ROC AUC score for the training dataset.
- **Test ROC AUC:** The ROC AUC score for the test dataset.

The ROC curves for both training and testing sets are plotted and saved as `roc_curve.png`.
