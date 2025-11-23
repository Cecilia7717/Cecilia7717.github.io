---
title: "Predicting Online Shopping Purchasing Intention Using Random Forest and AdaBoost Classifier"
order: 8
collection: projects
type: "REU project"
permalink: /projects/ml
venue: "Bryn Mawr College"
location: "Bryn Mawr, PA, USA"
paperurl: 'http://cecilia7717.github.io/files/ml.pdf'
---

Developed and evaluated supervised machine-learning classifiers with full preprocessing, tuning, 
and performance analysis to understand dataset behavior and improve predictive accuracy.

Overview
======

This machine learning project focuses on building and evaluating supervised classifiers to predict 
online shopping purchasing intentions using a dataset from the UCI Machine Learning Repository. 
I implemented logistic regression, decision trees, and ensemble methods such as random forests and AdaBoost, 
each integrated with standardized preprocessing pipelines and systematic hyperparameter tuning via GridSearchCV.
To understand model behavior, I generated validation curves that reveal how parameters like `n_estimators`, 
`learning_rate`, and `max_depth` affect overfitting and generalization—showing, for example, that AdaBoost p
erforms best with learning rates near 2e–2 and Random Forest stabilizes around 45 trees.

Model performance was evaluated using accuracy, precision, recall, F1 score, and confusion matrices. 
Consistent with the findings in the report, Random Forest achieved the highest precision, while AdaBoost
delivered stronger recall—indicating complementary strengths depending on whether reducing false positives 
or capturing more purchasers is prioritized. Feature importance analysis identified PageValues, ExitRates, 
and ProductRelated_Duration as the strongest predictors of purchase behavior, aligning with intuitions about user intent. 
All code and the full write-up are available on [GitHub](https://github.com/Cecilia7717/project-ml).
