# Semiconductor Analysis

**Goal/Objective:** 

Building a Supervised Machine Learning model that predicts the quality of a semiconductor wafer. Visualize patterns and perform Exploratory Data Analysis to make beneficial business decisions

**Data Pre-processing and Feature Engineering:**

The whole dataset had 592 columns making it hard to check every column so we used feature engineering method to select, manipulate and transform the raw data which could be later used for modelling purpose. The features in the dataset were all continuous/numeric and the response variable Pass.Fail is a categorical variable. None of the columns were missing but majority of the columns had missing data (41951 missing observations out of a total of 927664 observations.)

**Logistic Regression:**

The first classification approach was performed by logistic regression. Since logistic regression is probabilistic, prediction of probability that is related to class was possible. Therefore, we thought logistic regression can be good method to classify the target variable whether the class is "Pass" or "Fail". For the model implementation, Generalized Linear Model using 'glm' function and 'family = binomial' option were applied in R. After classification, it was able to see results of confusion matrices for both training and the test data and calculating of accuracy, specificity and sensitivity was also possible. Furthermore, bar plot was also available to compare the numbers of how many passes and fails from the model. 

Furthermore, K-Nearest Neighbor, Desicion Tree with Bagging, Random Forest with Boosting and Support Vector Machine were performed and their accuracies were compared and acheived as below: 

| **Method**                 | **Accuracy** | **Sensitivity** | **Specificity** |
|------------------------|----------|-------------|-------------|
| Logistic Regression    | 100%     | 1.000       | 1.000       |
| Decision Tree          | 100%     | 1.000       | 1.000       |
| Random Forest          | 100%     | 1.000       | 1.000       |
| Bagging/Boosting       | 100%     | 1.000       | 1.000       |
| Support Vector Machine | 99.04%   | 1.000       | 0.8500      |
| K-Nearest Neighbor     | 92.36%   | 0.9233      | 1.000       |
