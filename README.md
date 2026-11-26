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

**Key Performance Improvements & Observations**

1. Random Forest to Balanced Random Forest: Fraud recall improved from 59% to 73%, while fraud precision increased from 82% to 96%.
2. Random Forest to SMOTE + AdaBoost: Fraud recall increased from 59% to 91%, demonstrating substantially improved fraud identification, although precision decreased considerably.
3. Random Forest to SMOTE + Gradient Boosting: Fraud recall increased from 59% to 92%, with ROC-AUC improving from 0.9522 to 0.9794.
4. Best ROC-AUC: Gradient Boosting achieved 0.9794, indicating the strongest ranking performance among the evaluated models.

**Conclusion**

This project demonstrates how different ensemble learning strategies and class imbalance handling techniques influence fraud detection performance.
The experiments highlight that improving fraud detection recall does not necessarily improve precision or overall accuracy. Therefore, selecting an appropriate model requires balancing fraud detection capability with false-positive reduction.
The project provides practical exposure to developing, evaluating, and comparing multiple machine learning architectures for a real-world financial fraud detection problem.




