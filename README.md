# Statistical Modeling of Competitive Game Outcomes
**A Predictive Study on Pokémon Battle Success using R**

## 1. Project Overview
This project explores the relationship between base combat statistics and winning percentages in competitive gaming environments. Using a dataset of 800 observations, I developed a predictive pipeline to identify the primary drivers of success while maintaining strict adherence to Gauss-Markov assumptions.

## 2. Statistical Rigor & Validation
Unlike standard ML "black-box" approaches, this project emphasizes **statistical discipline**:
* **Multiple Linear Regression (OLS):** Achieved an **Adjusted R² of 0.902**.
* **Assumption Testing:** Conducted Shapiro-Wilk (Normality), Breusch-Pagan (Homoscedasticity), and VIF (Multicollinearity) tests.
* **Regularization:** Compared OLS against **Lasso and Ridge Regression** using 10-fold cross-validation to analyze the bias-variance tradeoff.

## 3. Key Findings
* **Primary Drivers:** Speed and Attack were identified as the most statistically significant predictors of a high win rate.
* **Model Selection:** While Lasso provided a sparser model, the OLS baseline was retained as it satisfied all theoretical assumptions and provided superior interpretability.

## 4. Repository Structure
* `data/`: Cleaned dataset used for modeling.
* `src/`: R-Markdown source code for the full analysis.
* `docs/`: Final technical report in PDF format.
