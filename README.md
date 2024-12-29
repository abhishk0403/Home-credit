# Home Credit Default Risk Prediction

This project focuses on predicting loan repayment behavior using the Home Credit dataset. The goal is to classify customers into two categories: those who are likely to repay their loans and those who may default.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Objective](#objective)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Conclusion](#conclusion)
- [Technologies Used](#technologies-used)
- [How to Use](#how-to-use)

---

## Project Overview
Lenders face challenges assessing the creditworthiness of applicants with limited credit histories. By leveraging the Home Credit dataset, this project uses machine learning techniques to improve risk prediction, benefiting both lenders and borrowers.

---

## Dataset
- **Source**: Home Credit Default Risk competition on Kaggle.
- **Size**: ~300,000 rows and ~120 columns.
- **Features**: Includes demographics, financial information, and previous loan records.
- **Target**: Binary classification (1 = Defaulter, 0 = Non-Defaulter).

---

## Objective
To build a model that predicts the probability of a customer defaulting on a loan, focusing on:
1. High accuracy.
2. Interpretability of results.
3. Robust handling of imbalanced data.

---

## Data Preprocessing
Key steps included:
- **Handling Missing Values**: Imputation for both numerical and categorical data.
- **Feature Engineering**: Created new features like debt-to-income ratio, number of credit cards, etc.
- **Scaling and Encoding**:
  - Scaled numerical data using StandardScaler.
  - Encoded categorical variables using One-Hot Encoding.
- **Data Balancing**: Addressed class imbalance using SMOTE and class weighting.

---

## Modeling
Several machine learning algorithms were employed:
1. Logistic Regression.
2. Decision Trees.
3. Random Forest.
4. LightGBM.
5. XGBoost.
6. AdaBoost.

The **LightGBM model** achieved the best performance with a ROC AUC score of **0.76**.

---

## Evaluation
- **Metrics Used**:
  - ROC AUC Score.
  - Precision, Recall, and F1-Score.
  - Confusion Matrix Analysis.
- The ROC AUC score of 0.76 indicates good discriminatory power.

---

## Conclusion
The project demonstrated how advanced machine learning techniques could improve loan risk prediction. The LightGBM model emerged as the best performer, balancing performance and efficiency.

---

## Technologies Used
- **Programming Language**: Python
- **Libraries**:
  - `pandas`, `numpy`, `matplotlib`, `seaborn` for EDA.
  - `scikit-learn` for preprocessing and modeling.
  - `LightGBM` and `XGBoost` for advanced modeling.
- **Tools**: Jupyter Notebook, GitHub.

---

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/home-credit-default-risk.git
   cd home-credit-default-risk
