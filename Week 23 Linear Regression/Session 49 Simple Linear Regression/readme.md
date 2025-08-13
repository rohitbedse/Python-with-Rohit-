# Session 49: Simple Linear Regression

## Overview
This repository provides learning materials and analysis for **Day 49: Simple Linear Regression** from the 100 Days of Machine Learning series.

## 1. What is Simple Linear Regression?
Simple Linear Regression (SLR) is a foundational supervised learning technique used to model the relationship between one independent variable \( x \) and one dependent variable \( y \), using a straight-line equation:

\[
y = m x + b
\]

- **\( m \)**: Slope or coefficient  
- **\( b \)**: Intercept (bias term)

---

## 2. Key Concepts Covered in Session 49

###  Model Training and Assessment
- Fit a straight line that best represents the relationship between input \( x \) and output \( y \).  
- Use **Mean Squared Error (MSE)** or **Root Mean Squared Error (RMSE)** to measure how well the model predicts.

###  Regression Metrics (From Day 49 GitHub)
- **MSE**: Average squared difference between observed and predicted values — lower is better.  
- **RMSE**: Square root of MSE — interpretable in original output units.  
- Potentially **Mean Absolute Error (MAE)** or **R² (Coefficient of Determination)** may also be introduced.

---

## 3. Learning Flow (Session 49)
1. **Concept Introduction**: Understanding the goal of SLR.  
2. **Deriving the Best-Fit Line**:
   - Closed-form solution using formulas (e.g., least squares method).  
   - Alternatively, using iterative methods like Gradient Descent for learning \( m \) and \( b \).  
3. **Implementation**:
   - Students execute code (via GitHub Day 48) to implement SLR from scratch or using libraries.  
4. **Evaluation**:
   - Apply regression metrics (from Day 49 materials) to evaluate performance.  
5. **Visualization**:
   - Plotting data points alongside the fitted regression line for intuitive understanding.

---

## 4. How to Use This Session’s Materials

1.  **Review Day 48 Code**: Understand the implementation of Simple Linear Regression ([Day 48 GitHub link](https://github.com/campusx-official/100-days-of-machine-learning/tree/main/day48-simple-linear-regression)).  
2.  **GitHub**: Focus on lessons around evaluating regression models using proper metrics ([Day 49 GitHub link](https://github.com/campusx-official/100-days-of-machine-learning/tree/main/day49-regression-metrics)).  
3.  **Download & Read Slides/Notes**: Use the [Google Drive PDF](https://drive.google.com/file/d/18oSjN8aEztz_m-_CoKb5i_kGHvKccjdp/view) for conceptual clarity and reference.  
4.  **Watch the Session Video**: Gain a complete walkthrough in [YouTube – Session 49](https://youtu.be/aEPoLeS6UMM?si=OvukeZjLLB6KFMoT).  
5.  **Practice**: Run code, tweak data, experiment with different metrics, and visualize outcomes.

---

## 5. Summary Table

| Component             | Description                                                              |
|----------------------|--------------------------------------------------------------------------|
| **Model**            | Simple Linear Regression (\( y = mx + b \))                              |
| **Metric(s)**        | MSE, RMSE (possibly MAE, R²) from Day 49 materials                       |
| **Code**             | Implementation details in GitHub Day 48 and Day 49 folders               |
| **Slides/Notes**     | Google Drive PDF explaining theory and examples                          |
| **Video Lecture**    | Complete session walk-through via YouTube                                |

---

**Next Steps:**
- After understanding SLR, move to **MLR (Multiple Linear Regression)** for more complex datasets.  
- Explore **regularization** techniques (like Ridge/Lasso) and **optimization** methods (like Gradient Descent).  
- Compare and contrast various regression metrics (e.g., MAE vs RMSE vs R²) on real datasets.

---
@rohitbedse_