# Data-Analysis-project
The aim of this research was to create and evaluate classifiers for predicting the "SpType-ELS" attribute in a given dataset. This project builds on a previous data exploration assignment and includes real data analytics tasks that are typical of a data scientist's position in a consultancy. The primary goal was to thoroughly preprocess the data, apply several classification approaches, modify their parameters, and select the best performing model in a logical and explainable manner.
Project Workflow
Data Preprocessing

Data preprocessing involved handling missing values, scaling features, and discretizing continuous variables. The following pipelines were used:

    Standard Scaling Pipeline: Imputes missing values with the mean and applies standard scaling.
    Min-Max Scaling Pipeline: Imputes missing values with the mean and applies min-max scaling.
    Discretization Pipeline: Imputes missing values with the mean and discretizes features like "Teff" and "Age-Flame" using KBinsDiscretizer with k-means strategy.
    Categorical Encoding Pipeline: Encodes categorical variables using OrdinalEncoder.

Model Building and Evaluation

Various classifiers were built using the processed data, including:

    GaussianNB
    GradientBoostingClassifier
    DecisionTreeClassifier

Each model's hyperparameters were tuned using GridSearchCV to find the optimal settings. Performance was evaluated based on precision, recall, F1-score, and AUC score.
Best Classifier Selection

The GradientBoostingClassifier was selected as the best classifier due to its outstanding performance:

    Precision: 0.99
    F1-score: 0.99
    Recall: 0.99
    AUC score: 0.9996

This model effectively combined the outputs of multiple weak learners to create a strong overall classifier, making it the most suitable choice for this task.
Submission

Predictions on the unknown dataset were formatted according to the sample submission file and submitted to the Kaggle competition.
