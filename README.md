# Liver-Disease-Prediction
Build and compare ML models to predict liver disease accurately, assisting in early detection and clinical decision-making.
# Data Preprocessing

Handling Missing Values: Checked and removed/fixed missing entries.

Encoding Categorical Variables: Gender encoded as 0 (Female) and 1 (Male).

Feature Scaling: Standardized numeric features for SVC and Logistic Regression.

Train-Test Split: 80% training, 20% testing data.
# Machine Learning Models

We applied three models:

5.1 Logistic Regression (LR)

Linear model for binary classification.

Interpretable coefficients showing feature impact.

5.2 Support Vector Classifier (SVC)

Finds the optimal hyperplane separating two classes.

Effective for high-dimensional data.

5.3 Random Forest Classifier (RF)

Ensemble of decision trees using majority voting.
Random Forest performed best in all metrics, followed closely by SVC. Logistic Regression provides interpretability but slightly lower accuracy.
# Model Evaluation

Confusion Matrix: Random Forest correctly predicted the majority of liver disease cases.

ROC-AUC: Random Forest: 0.85, SVC: 0.82, Logistic Regression: 0.80

Cross-Validation: 5-fold cross-validation confirms model stability and reliability.
# Observations:

Logistic Regression has the highest overall accuracy (73.5%) and slightly lower recall compared to SVC and Random Forest.

SVC and Random Forest achieved perfect recall (100%), meaning they correctly identified all liver disease cases, but their accuracy is slightly lower (70.9%) due to some false positives.

F1-Score balances precision and recall: Logistic Regression has a slightly better F1-score (0.836), indicating good balance between detecting liver disease and avoiding false alarms.
# Conclusion:

If detecting all actual liver disease cases is the priority (medical screening scenario), SVC or Random Forest are preferable.

If overall balanced performance is preferred, Logistic Regression is slightly better due to higher F1-score and accuracy.


Handles non-linear relationships and reduces overfitting.
