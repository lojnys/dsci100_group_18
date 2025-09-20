# Classification of User Knowledge Project (DSCI 100)

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
|**KNN Classification**|**0.3379**|

With hyperparameter tuning with cross-validation, we were able to get an accuracy of 0.3379.

## Results & Findings

This study applied a K-nearest neighbour (KNN) algorithm with k=5 to predict students’ knowledge levels using two variables: degree of study time (STG) and degree of repetition (SCG). The model achieved an accuracy of only 0.3379, indicating that these predictors were weakly related to knowledge levels and led to poor classification performance. While the expectation was that higher study time and repetition would correspond to higher knowledge, this was not observed. The low accuracy suggests that more relevant variables or alternative classification algorithms are needed to better capture the factors influencing knowledge. Despite its limitations, a successful KNN model could still be valuable for identifying at-risk students early and guiding interventions, but in this case, the choice of predictors limited its effectiveness.

## References
-Agarwal, T. (2020, October 31). DC machine - construction, working, types, EMF Equation & Applications. ElProCus. https://www.elprocus.com/dc-machine-types-and-their-applications/#:~:text=A%20DC%20machine%20is%20an,that%20rotates%20the%20dc%20motor 

-Bartoszewski, B. L., & Gurung, R. A. (2015). Comparing the relationship of learning techniques and exam score. Scholarship of Teaching and Learning in Psychology, 1(3), 219–228. https://doi.org/10.1037/stl0000036

-Deeva, G., De Smedt, J., Saint-Pierre, C., Weber, R. W., & De Weerdt, J. (2022). Predicting student performance using sequence classification with time-based windows. Expert Systems With Applications, 209, 118182. https://doi.org/10.1016/j.eswa.2022.118182

-Dunlosky, J., Rawson, K. A., Marsh, E. J., Nathan, M. J., & Willingham, D. T. (2013). Improving students’ learning with effective learning techniques. Psychological Science in the Public Interest, 14(1), 4–58. https://doi.org/10.1177/1529100612453266

-I. A. Abu Amra and A. Y. A. Maghari, "Students performance prediction using KNN and Naïve Bayesian," 2017 8th International Conference on Information Technology (ICIT), Amman, Jordan, 2017, pp. 909-913, doi: 10.1109/ICITECH.2017.8079967.

-Schneider, J. (2017). Wrong Answer: Standardized Tests and Their Limitations. In Beyond test scores: A better way to measure school quality (pp. 14–51). essay, Harvard University Press
