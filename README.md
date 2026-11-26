# Credit-Card-Fraud-Detection

**comparative evaluation of Bagging, Boosting, and Stacking approaches, along with class imbalance handling using class_weight and SMOTE**

Developed an end-to-end Credit Card Fraud Detection system using multiple Machine Learning and Ensemble Learning techniques to identify fraudulent transactions in a highly imbalanced dataset. The project explores Bagging, Boosting, and Stacking algorithms, incorporating class imbalance handling techniques to improve fraud detection performance while evaluating the trade-off between precision, recall, F1-score, and overall accuracy. Rather than relying on accuracy alone, the project focuses on improving the identification of minority-class (fraudulent) transactions.

**Dataset & Preprocessing**
Dataset: Credit Card Transactions
Total transactions: 284,807
Features: 30 input features
Target variable: Class (0 = Legitimate, 1 = Fraudulent)
Train-Test Split: 80:20 with stratification.
Missing Value Analysis: Checked for missing values.
Feature Scaling: StandardScaler applied to training and testing datasets.

**Machine Learning Techniques Implemented**

1. Random Forest – Bagging Ensemble
2. Class Weight Balancing – Imbalance Handling
3. SMOTE – Synthetic Minority Oversampling
4. AdaBoost – Boosting Ensemble
5. Gradient Boosting – Boosting Ensemble
6. Stacking Classifier – Multi-Level Ensemble Learning

**Model Performance Comparison**
The following results were obtained from the notebook's test-set evaluation.

Model                          Accuracy              Precision (Fraud)                Recall (Fraud)                 F1-score
Random Forest                   99.91%                    82%                            59%                          0.69
Balanced Random Forest          99.95%                    96%                            73%                          0.83
SMOTE + AdaBoost                98.13%                     8%                            91%                          0.14
SMOTE + Gradient Boosting       98.02%                     7%                            92%                          0.14

**ROC-AUC Comparison**
  
  Model                          ROC-AUC
Random Forest                    0.9522
Balanced Random Forest           0.9534
SMOTE + AdaBoost                 0.9712
SMOTE + Gradient Boosting        0.9794

**Conclusion**

This project demonstrates how different ensemble learning strategies and class imbalance handling techniques influence fraud detection performance.
The experiments highlight that improving fraud detection recall does not necessarily improve precision or overall accuracy. Therefore, selecting an appropriate model requires balancing fraud detection capability with false-positive reduction.
The project provides practical exposure to developing, evaluating, and comparing multiple machine learning architectures for a real-world financial fraud detection problem.




