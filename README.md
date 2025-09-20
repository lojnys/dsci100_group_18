# Classification of User Knowledge Project (DSCI 10

## Authors
- Kyrstin Lavelle
- Yushin Nam
- Accita Ongko
- Krianna Strowbridge

## Problem Statement
- **Goal**: The primary objective is to build a classification model that predicts students' knowledge levels based on the features given, with appropriate feature selection analytically.
- **Metric used**: The model's performance will be evaluated based on its **accuracy** score. 

## Dataset
- **Source**: The dataset was obtained from UCI Machine Learning Repository. [https://archive.ics.uci.edu/dataset/257/user+knowledge+modeling]
- Description: The data contains 403 instances with 5 features; STG, SCG, STR, LPR, PEG, and UNS; UNS being the target variable. The other four attributes includes information about each student's study routine and behaviour.This dataset does not contain any missing values.

|Feature|Description|Data type|
|---|---|---|
|STG|The degree of study time for goal object materials|Continous|
|SCG|The degree of repetition number of user for goal object materials|Continuous|
|STR|The degree of study time of user for related objects with goal object|Continuous|
|LPR|The exam performance of user for related objects with goal object|Continuous|
|PEG|The exam performance of user for goal objects|Continuous|
|UNS|The knowledge level of user|Categorical|

## Modeling & Evaluation

Only one classification model was trained and evaluated in the scope of DSCI 100. 

|Model|Accuracy|
|---|---|
|KNN Classification|0.3379|

With hyperparameter tuning with cross-validation, we were able to get an accuracy of 0.3379. For deeper discussion, take a look at *group_report.ipynb* under *Discussion*.
