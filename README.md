# Bank-customers-behavior-prediction

## Overview
This project applies machine learning techniques to analyze and predict customer behavior for bank marketing campaigns using the Bank Marketing Dataset. The primary goal is to identify potential customers likely to subscribe to a long-term deposit, thereby optimizing marketing efforts and strategies.

---

## Dataset Description
The dataset used in this project was sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing) and contains 45,211 samples with 17 features, including:

- **Customer Attributes:** age, job, marital status, education, etc.
- **Campaign Details:** duration of calls, contact method, number of contacts, etc.
- **Target Variable (y):** Whether a customer subscribed to a term deposit (`yes` or `no`).

The dataset is imbalanced, with the majority class (`no`) significantly outweighing the minority class (`yes`).

---

## Project Objectives
1. Build predictive models to classify whether a customer will subscribe to a term deposit.
2. Improve model performance by addressing data imbalance.
3. Evaluate models using metrics such as precision and recall.

---

## Data Preprocessing
To prepare the dataset for machine learning, the following steps were performed:
1. **Exploratory Data Analysis (EDA):**
   - Correlation analysis revealed that the `duration` feature had a high correlation with the target variable.
   - Visualization of customer behavior trends based on age, balance, and number of contacts.
2. **Handling Imbalanced Data:**
   - Applied techniques like Random Undersampling, SMOTE, and ADASYN to balance the target variable.

---

## Machine Learning Models
The following models were implemented and evaluated:
1. **Logistic Regression**
   - Strengths: Interpretable coefficients and efficient for large datasets.
2. **Naive Bayes**
   - Gaussian Naive Bayes was used for its simplicity and effectiveness with continuous features.
3. **Random Forest**
   - An ensemble model that combines multiple decision trees for robust predictions.
4. **CatBoost Classifier**
   - Gradient boosting-based model optimized for categorical and numerical features.

---

## Results
The results demonstrated that:
- **Random Forest with Random Undersampling** achieved the highest recall (89%) and precision (42%).
- Other models like CatBoost and Logistic Regression also performed well with balanced datasets.

| Model                | Precision | Recall |
|----------------------|-----------|--------|
| Logistic Regression | 0.37      | 0.77   |
| Naive Bayes         | 0.27      | 0.82   |
| Random Forest       | 0.42      | 0.89   |
| CatBoost            | 0.42      | 0.88   |

---

## Future Work
- Explore advanced data augmentation techniques to address class imbalance.
- Implement neural network models for better feature extraction and performance.
---

## References
1. Moro, S., Laureano, R., & Cortez, P. (2011). Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology.
2. [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing)
