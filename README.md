# Brazilian E-Commerce (Olist) Data Analysis

## Project Overview
This project analyzes the relationship between customer review scores and product return rates using the Brazilian E-Commerce Public Dataset (Olist) from Kaggle. The goal is to identify whether low review scores are associated with higher return rates, understand patterns by product category, and apply machine learning to predict returns.

## Key Questions
1. Are lower review scores associated with higher return rates?
2. Do certain product categories have higher return rates?
3. Are return rates different by season or delivery time?

## Methodology
- **Data Preprocessing**: Merging datasets to create a unified analysis table
- **Exploratory Data Analysis (EDA)**: Descriptive statistics, visualizations, correlation analysis
- **Statistical Testing**:
  - T-test between low and high score groups
  - ANOVA across product categories
  - Chi-square test of independence
- **Regression**:
  - Simple & Multiple Linear Regression (with `review_score`, `delivery_late`, `total_price`)
- **Modeling**:
  - Logistic Regression
  - Random Forest with SMOTE to handle class imbalance

## Key Findings
- Weak negative correlation between review score and return status (r = -0.12)
- T-test and regression confirmed statistically significant difference in return rate between low and high review scores
- Chi-square test revealed product category and return rate are related
- Final Random Forest model (after SMOTE):
  - **Accuracy**: 95%
  - **Recall (for returns)**: 65%
  - **Precision**: 6%

## Tech Stack
- Python (Pandas, NumPy, Seaborn, Scikit-learn, Statsmodels)
- Jupyter Notebook
- imbalanced-learn (SMOTE)

## 📁 Project Structure
```
Olist_Return_Prediction/
├── data/                    # (Optional) data samples or metadata
├── images/                  # (Optional) visualizations
└── notebooks/
    ├── olist_return_analysis.ipynb
    └── olist_return_analysis.html
```

## Dataset Source
[Kaggle - Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## Author
Yoonji Choi  
Contact: [your.email@gmail.com]  
GitHub: [https://github.com/your-username](https://github.com/your-username)

**This project is shared for portfolio viewing only. Do not copy, modify, or redistribute.**
