# 📊 Session 43 – Central Limit Theorem (CLT)

## 🔍 What You Learned:
**Central Limit Theorem (CLT)** is the backbone of inferential statistics.  
It explains how sampling distributions behave and why we can use the normal distribution even when the data itself is not normal.

---

## 🧠 Central Limit Theorem – Key Idea:
> When you take **random samples** from any population and compute their means,  
> the **distribution of those sample means tends to be normal**, **as sample size increases** – regardless of the population’s shape.

---

## 🧪 Key Concepts Covered:

| Topic                     | Description                                 |
|--------------------------|---------------------------------------------|
| Population vs Sample     | Focus on averages from multiple samples      |
| Sampling Distribution     | Distribution of sample means                |
| Law of Large Numbers     | Larger samples give more stable estimates   |
| Importance in ML/Stats   | Basis for confidence intervals & hypothesis |

---

## 🛠️ Resources Used:

- 📺 [YouTube Session](https://www.youtube.com/live/-WmJDYBor7c?si=JvT_V-qqd6CXqwn8)
- 📓 [Colab Notebook](https://colab.research.google.com/drive/1W--4mte3uaDD8rReLAt4OWEoLXrb5Ij7?usp=sharing)
- 📘 [PDF Notes](https://drive.google.com/file/d/14izghg0Aw5v3ed1rq9xEHZVcG_x0hMD-/view)
- 📊 [Kaggle Notebook (Titanic CLT Demo)](https://www.kaggle.com/code/campusx/titanic-clt)

---

## 📈 Real-Life Applications:
- Estimate average height, income, age, etc.
- Calculate confidence intervals
- Base for A/B testing
- Statistical inference even with non-normal raw data

---

## 🧪 Sample Size Matters:
| Sample Size (n) | Shape of Sample Mean Distribution |
|-----------------|-----------------------------------|
| Small (n=5)     | May still look skewed             |
| Medium (n=30)   | Starts to resemble normal          |
| Large (n=50+)   | Becomes nearly normal              |

---

## ✅ Pro Tip:

Use Python to simulate CLT:
```python
import numpy as np
means = [np.mean(np.random.choice(data, size=30)) for _ in range(1000)]
plt.hist(means, bins=30)

@rohitbedse_