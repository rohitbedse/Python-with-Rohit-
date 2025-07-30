# 📊 Session 44 – Confidence Interval (CI)

## 🔍 What You Learned:
**Confidence Intervals** give us a range of values where the **true population parameter** (like mean) is likely to lie, based on sample data.

---

## 📌 Confidence Interval – Basic Idea:

> Instead of giving a **single estimate**, we give a **range** (interval) with a **confidence level** (like 95%).

For example:  
**"The average height is between 160 cm and 170 cm with 95% confidence."**

---

## 🧠 Formula (when population std. dev is known):

\[
CI = \bar{x} \pm z \cdot \frac{\sigma}{\sqrt{n}}
\]

Where:
- \( \bar{x} \) = sample mean  
- \( z \) = z-score (e.g., 1.96 for 95%)  
- \( \sigma \) = population standard deviation  
- \( n \) = sample size

---

## 🛠️ Resources Used:

- 📺 [YouTube Session](https://www.youtube.com/live/X52HK2qkiIE?si=r55lm4USLeCrSsVx)
- 📘 [PDF Notes](https://drive.google.com/file/d/1nskWHtR1ePmrje76k71gdUc2-fcVWvMH/view?usp=share_link)

---

## 📈 Common Confidence Levels:

| Confidence Level | Z-Value |
|------------------|---------|
| 90%              | 1.645   |
| 95%              | 1.96    |
| 99%              | 2.576   |

---

## 📌 Use Cases of Confidence Intervals:

- Estimating average income, height, marks, etc.  
- Polling results (e.g., "support is 52% ± 3%")  
- Error margin in experiments  
- Clinical trial outcomes

---

## ✅ Pro Tip (Python):

```python
from scipy import stats
import numpy as np

sample = [random data]
mean = np.mean(sample)
sem = stats.sem(sample)
ci = stats.t.interval(0.95, len(sample)-1, loc=mean, scale=sem)
print("95% Confidence Interval:", ci)

@rohitbedse_