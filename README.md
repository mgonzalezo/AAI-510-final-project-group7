# AAI-510 Final Team Project - Team 7
## Predicting Customer Churn in Telecommunications Using Machine Learning

**Course:** AAI-510 Introduction to Artificial Intelligence  
**University of San Diego — Applied Artificial Intelligence (MS)**  
**Team 7:** Marco Gonzalez Ortiz, Harsh Modi, Aishwarya Pareek  
**Date:** June 2026

---

## Project Overview

Customer churn is one of the most critical challenges in the telecommunications industry. This project builds a predictive machine learning model that identifies customers at high risk of churning, enabling proactive retention strategies that reduce attrition and increase customer lifetime value.

We use the [Telco Customer Churn dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) (7,043 records) and compare three classification algorithms — Logistic Regression, Random Forest, and Gradient Boosting — with hyperparameter tuning and threshold optimization for business-relevant decision making.

## Repository Contents

| File | Description |
|------|-------------|
| `Team7_AAI_510_FinalTeamProject.ipynb` | Jupyter Notebook with full analysis, modeling, and evaluation |

## Methodology

The project follows the CRISP-DM framework:

1. **Business Understanding** — Define the churn prediction problem and its financial impact
2. **Data Understanding** — Exploratory data analysis with graphical and non-graphical methods
3. **Data Preparation** — Cleaning, encoding, scaling, and stratified train/test split
4. **Feature Selection** — Analysis-driven feature inclusion with multicollinearity handling
5. **Modeling** — Three models trained with GridSearchCV (Logistic Regression, Random Forest, Gradient Boosting)
6. **Evaluation** — ROC-AUC, Precision-Recall, confusion matrix, feature importance
7. **Deployment** — Batch inference architecture with monitoring and retraining strategy

## Key Findings

- **Tenure** is the strongest predictor of churn — new customers (0-6 months) are at highest risk
- **Month-to-month contracts** drive the majority of churn; contract upgrades are the most actionable lever
- **Tech Support gaps** significantly increase churn probability
- The optimized model catches ~75% of churners with an actionable precision level

## How to Run

1. Upload the notebook to [Google Colab](https://colab.research.google.com/)
2. Upload the dataset (`WA_Fn-UseC_-Telco-Customer-Churn.csv`) from [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) to `/content/`
3. Run all cells sequentially

## AI Tools Disclosure

AI-assisted tools (Claude, GitHub Copilot) were used to accelerate code development and review report structure. All model selection decisions, business interpretations, and recommendations were made by the team.
