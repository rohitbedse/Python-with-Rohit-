# Session 50: Multiple Linear Regression (MLR)

## Overview
This document summarizes the concepts and practice materials for **Day 50: Multiple Linear Regression**, part of the *100 Days of Machine Learning* series.

---

## Resources
- 📓 **MLR with Libraries**: [multiple_linear_regression.ipynb](https://colab.research.google.com/github/campusx-official/100-days-of-machine-learning/blob/main/day50-multiple-linear-regression/multiple_linear_regression.ipynb#scrollTo=NpAvnU-t3yV0)  
- 📓 **MLR from Scratch**: [code-from-scratch.ipynb](https://colab.research.google.com/github/campusx-official/100-days-of-machine-learning/blob/main/day50-multiple-linear-regression/code-from-scratch.ipynb#scrollTo=afc9a715)  
- 🎥 **Live Session Video**: [YouTube – Session 50](https://www.youtube.com/live/e_9vJXokd-Y?si=0KVN6QEOx4YubyGG)  
- 📄 **Supplemental Slides/Notes**: [Google Drive PDF](https://drive.google.com/file/d/1fYGa7wXCirq8Tvo2YqfHsQSlhs1DXXwo/view)

---

## 1. What is Multiple Linear Regression?
Multiple Linear Regression is a supervised learning technique used to model the relationship between one dependent variable \( y \) and multiple independent variables \( x_1, x_2, ..., x_n \).  

**General equation:**
\[
y = b_0 + b_1 x_1 + b_2 x_2 + \dots + b_n x_n
\]
- \( b_0 \) → Intercept  
- \( b_1, b_2, ..., b_n \) → Coefficients (weights)  

---

## 2. Key Topics Covered
- Concept of extending linear regression to multiple features.
- Interpretation of coefficients in multi-feature scenarios.
- Model fitting using:
  - **Closed-form solution** (Normal Equation)
  - **Gradient Descent** optimization
- Evaluating performance using metrics like:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Coefficient of Determination (\( R^2 \))
- Importance of scaling features for gradient-based methods.
- Visualizing regression planes and residuals.

---

## 3. Learning Flow
1. **Understand the Theory** – Learn how multiple predictors affect the outcome and how coefficients are estimated.  
2. **Implementation with Libraries** – Train and test MLR models using ready-made functions (e.g., scikit-learn).  
3. **Implementation from Scratch** – Code the math manually to see how weight updates occur.  
4. **Model Evaluation** – Use regression metrics to assess model quality.  
5. **Practice** – Apply the method to datasets with varying numbers of features.

---

## 4. Suggested Next Steps
- Explore **Polynomial Regression** to capture non-linear patterns.
- Apply **Regularization** techniques (Ridge, Lasso, Elastic Net) to reduce overfitting.
- Experiment with **feature selection** to identify the most impactful variables.
- Use cross-validation to get a more reliable estimate of model performance.

---

@rohitbedse_
