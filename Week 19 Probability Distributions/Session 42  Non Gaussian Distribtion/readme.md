# 📊 Session 42 – Non-Gaussian Distributions (Quick Summary)

## 🔍 What You Learned:
Not all real-world data follows a **normal distribution**.  
In this session, we explored different types of **non-Gaussian distributions** and how to transform them.

---

## 🌀 Types of Non-Gaussian Distributions:

| Distribution Type      | Description                               |
|------------------------|-------------------------------------------|
| **Right-Skewed**       | Long tail on right side (e.g., income)    |
| **Left-Skewed**        | Long tail on left side                    |
| **Bimodal**            | Two peaks (e.g., height of children+adults) |
| **Uniform**            | Constant probability across range         |
| **Exponential**        | Decay-type distribution (e.g., waiting time) |

---

## 🔧 Data Transformation Techniques:

### 1. **FunctionTransformer** (Log, Square-root, etc.)
- Use to stabilize variance, reduce skewness
- ⚙️ Resource: [Function Transformer GitHub](https://github.com/campusx-official/100-days-of-machine-learning/tree/main/day30-function-transformer)

### 2. **PowerTransformer (Box-Cox / Yeo-Johnson)**
- Automatically makes data more Gaussian-like
- ⚙️ Resource: [Power Transformer GitHub](https://github.com/campusx-official/100-days-of-machine-learning/tree/main/day31-power-transformer)

---

## 🛠️ Resources Used:

- 📺 [YouTube Session](https://youtu.be/U6QCc_3zgUk?si=AzOJLuF8iOPYxAum)
- 📓 [Colab Notebook](https://colab.research.google.com/drive/1Q2ug8BXogFqYY_6e04dmHk0Tn5_yfObo?usp=sharing)
- 📘 [PDF Notes](https://drive.google.com/file/d/1sd4nz8PNsGc334ng86V8uKvJNqhWyRZ2/view)
- 🛠️ [Function Transformer GitHub](https://github.com/campusx-official/100-days-of-machine-learning/tree/main/day30-function-transformer)
- ⚙️ [Power Transformer GitHub](https://github.com/campusx-official/100-days-of-machine-learning/tree/main/day31-power-transformer)

---

## 📈 Real-World Examples:
- **Right-skewed**: Income, Housing Prices  
- **Left-skewed**: Age at retirement  
- **Exponential**: Time until machine failure  
- **Bimodal**: Heights (men & women), test scores (pass vs fail)

---

## 🧠 Why It’s Important:
- Many ML models (like Linear Regression, Logistic Regression) assume **normality**  
- Applying transformations helps:
  - Improve **model accuracy**
  - Reduce **bias**
  - Stabilize **variance**

---

## ✅ Pro Tip:

Use `sklearn.preprocessing.PowerTransformer` for automatic normalization:
```python
from sklearn.preprocessing import PowerTransformer
pt = PowerTransformer()
X_transformed = pt.fit_transform(X)


@rohitbedse_

