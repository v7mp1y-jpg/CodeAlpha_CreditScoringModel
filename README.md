# CodeAlpha - Credit Scoring Model

##  Task Overview
This project was developed as part of the CodeAlpha Machine Learning Internship (Task 1: Credit Scoring Model).

The objective is to predict whether a customer will default on credit payment using historical financial and repayment data.

---

##  Dataset
Dataset: Default of Credit Card Clients  
Source: UCI / Public GitHub Dataset  
Target Variable: `default_payment_next_month`  
- 0 → No Default  
- 1 → Default  

---

##  Preprocessing Steps
- Cleaned column names
- Handled missing values using median imputation
- Standardized numerical features using StandardScaler
- Addressed class imbalance using class weights
- Stratified train-test split (80/20)

---

##  Models Implemented
1. Logistic Regression
2. Decision Tree
3. Random Forest

---

##  Evaluation Metrics
Models were evaluated using:
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix
- ROC Curve

---

##  Results Summary

| Model              | Precision (1) | Recall (1) | F1 (1) | ROC-AUC |
|--------------------|---------------|------------|--------|---------|
| Logistic Regression| 0.369        | 0.622      | 0.463  | 0.708   |
| Decision Tree      | 0.402        | 0.396      | 0.399  | 0.614   |
| Random Forest      | 0.656        | 0.340      | 0.448  | 0.764   |

- **Best ROC-AUC:** Random Forest (0.764)
- **Best Recall for Default Detection:** Logistic Regression (0.622)

---

##  Conclusion
Random Forest achieved the highest ROC-AUC, indicating strong ranking ability for credit risk assessment. Logistic Regression achieved higher recall for detecting defaulters, making it suitable when minimizing financial risk is prioritized.

---

##  Saved Model
The best-performing model pipeline is saved as:

`best_credit_scoring_pipeline.joblib`

---

##  How to Run
pip install pandas numpy scikit-learn matplotlib joblib


## 2. Run the notebook or script:
CreditScoringModel.ipynb

## 3. Author
Farhan Ali  
CodeAlpha Machine Learning Internship
