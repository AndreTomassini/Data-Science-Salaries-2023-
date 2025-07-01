# Data-Science-Salaries-2023-
This repository analyzes the “Data Science Salaries 2023” dataset from Kaggle, exploring salary trends by experience level, remote work ratio, company size, and location. The project includes EDA, visualizations, regression models, and AI-assisted insights to guide career decisions in the data industry.

## 🔍 Objective

As Data Science students entering the job market, our motivation was to analyze how different factors—such as remote work ratio, company location, pay currency, and experience level—affect compensation in the global data industry. The goal is to support better-informed career decisions and enhance salary negotiation strategies in this evolving field.

## 📦 About the Dataset

- Dataset Source: Kaggle – "Data Science Salaries 2023"
- The dataset includes information on over 3,000 data professionals worldwide.
- Key features include job title, experience level, employment type, salary (in USD), remote ratio, company location, and company size.
- Motivation: Understand what impacts salary variation in the data science industry, a relevant topic for students preparing to enter this market.

## 🧹 Data Cleaning

- Removed over 1,500 duplicate entries.
- Addressed missing values (though the dataset was mostly clean).
- Converted appropriate columns to categorical or numerical types:
  - E.g., `experience_level`, `company_location`, and `company_size` converted to categorical types for better analysis.
  - `salary` converted to float for numerical operations.

## 📊 Exploratory Data Analysis (EDA)

- Used `describe()` to understand basic statistical properties.
- Performed visual exploration using:
  - **Boxplots** to compare salary distributions across experience levels.
  - **Regression plots** to examine the effect of remote work and job features on salary.
  - **Correlation matrix** to identify the strongest predictors of salary.
  - **Heatmap** to explore salary variations across company size and location.
- Insights revealed salary increases with experience and larger company sizes. Full-remote roles also tended to pay more.

## 🔎 Modeling & Evaluation

Implemented and compared three models:

1. **Linear Regression**  
   - Baseline model using one key feature (e.g., experience level).
   - R² ≈ 0.24

2. **Polynomial Regression (degree 2)**  
   - Added non-linearity and more features like experience, remote ratio, and job title.
   - Best configuration reached R² ≈ 0.33

3. **Ridge Regression with GridSearchCV**  
   - Regularized model tested across multiple alpha values using cross-validation.
   - R² ≈ 0.23

- All models showed moderate performance. This suggests that external factors—such as macroeconomic indicators, company revenue, or negotiation skills—might significantly impact salary but aren't captured in the dataset.
- Visual model comparisons were made using line plots over scatter plots for interpretability.

## 💡 Insights & Conclusions

- Experience level and company size have the strongest relationship with salary.
- Remote ratio also has a positive impact: full-remote jobs tend to pay more.
- Models alone cannot fully predict salary—real-world dynamics like company reputation, location-specific cost of living, and job demand play major roles.
- Understanding these trends helps students tailor their skills and job strategies.

## 🤖 AI Collaboration

This project integrated Generative AI (ChatGPT) to:
- Guide through the entire process: cleaning, visualization, and modeling.
- Suggest and improve Python code.
---

*Developed as part of the Master's in Data Science program at Southeastern University.*
