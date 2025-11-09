# Credit_card_fraud_detection
A machine learning framework using Logistic Regression, Random Forest, and XGBoost to detect credit card fraud in real time. Built on the Kaggle dataset, it delivers scalable, explainable, and business-ready risk scoring for banks and financial institutions.

# Key Findings

The dataset contained high class imbalance (fraud cases < 1% of total transactions).

After applying SMOTE, the fraud-to-non-fraud ratio improved, allowing models to learn fraudulent patterns better.

Amount and certain transformed features (like anonymized PCA components / Time) showed noticeable differences between fraudulent and normal transactions.

Models such as Logistic Regression, Random Forest, and XGBoost were trained and evaluated using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.

XGBoost performed best with the strongest balance between detecting frauds and avoiding false alarms.

# Interpretation of Model Results 
Logistic Regression

Very simple and fast to train.

Works well when data has linear patterns.

However, it missed many fraud cases because fraud patterns are complex and non-linear.

Interpretation: Logistic Regression is not suitable for fraud detection when patterns are hidden and imbalanced.

Random Forest

Able to detect more fraudulent transactions than Logistic Regression.

Produces lower false positives, meaning genuine customers are less likely to be flagged.

Slightly slower because it uses multiple decision trees.

Interpretation: Fraud transactions follow non-linear relationships, and Random Forest captures them better.

XGBoost (Best Performing Model)

Achieved the highest recall, meaning it caught most fraud cases.

Good precision—fewer wrong fraud predictions.

Best ROC-AUC score, showing strong classification ability.

# Conclusion

The project successfully demonstrated how machine learning can detect fraudulent credit card transactions.

Handling class imbalance (SMOTE) was critical—without it, models ignored fraud instances.

Among all models, XGBoost delivered the highest accuracy and recall, making it the most suitable for real-world fraud detection.

The model can help banks:
Reduce financial loss
Flag suspicious transactions in real time Improve customer safety

In real deployment, this model can be integrated with live transaction systems and continuously retrained as fraud patterns change.

Works well even with imbalanced datasets.

Interpretation: XGBoost is the most effective model because it learns complex fraud patterns by boosting weak learners and reducing errors.
