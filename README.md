# 🎓 Ivy League Admission Predictor – Jamboree Regression Project

This project aims to predict the probability of admission to Ivy League graduate programs based on Indian applicants' profiles. The model was developed in collaboration with Jamboree, a leading admissions consultancy.

## 📌 Objective

- Predict chances of admission (`Chance of Admit`) using features like GRE, TOEFL, GPA, etc.
- Understand key predictors and provide data-backed admission guidance.
- Evaluate models using metrics like R², RMSE, and MAE.

## 🔍 Dataset

- **Features**:
  - GRE Score
  - TOEFL Score
  - University Rating
  - SOP & LOR Scores
  - Undergraduate GPA
  - Research Experience

## 🔧 Methodology

- **EDA**: Univariate, Bivariate & Multivariate analysis
- **Feature Engineering**:
  - Standardization using `StandardScaler`
  - Dropped insignificant features (e.g., SOP)
  - Multicollinearity check using VIF
- **Modeling**:
  - Linear Regression
  - Lasso & Ridge Regularization
  - Cross-validation (5-fold)

## 📈 Results

| Model           | R²    | RMSE   |
|----------------|-------|--------|
| Linear (All)   | 0.818 | 0.0609 |
| Lasso (Best α) | 0.819 | 0.0608 |

- GPA and GRE were the most influential predictors.
- Lasso slightly outperformed Ridge due to feature selection benefits.

## 📊 Key Insights

- GPA has the strongest impact on admission chances.
- SOP was statistically insignificant and safely excluded.
- Research experience and LOR added marginal improvements.

## 📌 Future Enhancements

- Incorporate nonlinear models (e.g., XGBoost, SVR)
- Add interaction terms and SHAP interpretability
- Extend with real applicant outcomes as feedback loop

---

Project by Gargi Mishra
