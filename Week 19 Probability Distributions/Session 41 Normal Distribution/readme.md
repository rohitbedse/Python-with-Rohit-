# 📊 Session 41 – Normal Distribution (Quick Summary)

## 🔍 What You Learned:
- Normal distribution is a **bell-shaped** curve
- Defined by **mean (μ)** and **standard deviation (σ)**
- **Z-score formula**:
  z = (x - μ) / σ


---

## 📌 68-95-99.7 Rule (Empirical Rule)

| Range            | Coverage     |
|------------------|--------------|
| μ ± 1σ           | 68% data     |
| μ ± 2σ           | 95% data     |
| μ ± 3σ           | 99.7% data   |

---

## 🛠️ Resources Used:

- 📺 [YouTube Session](https://www.youtube.com/live/ADqYqSdtyW8?si=otgESgtA627iID_S)
- 📓 [Colab Notebook](https://colab.research.google.com/drive/1N_T0_w5vpT1k1Z4pSf4IMhAxYT1nRKLU?usp=sharing)
- 🌐 [Streamlit Visualizer App](https://samp-suman-normal-dist-visualize-app-lkntug.streamlit.app/)
- 📘 [PDF Notes / Slides](https://drive.google.com/file/d/11V7c5D80UDteolb_DVgS0em72pfMB-i0/view)
- 🧮 [Z-Table](https://www.ztable.net/)

---

## 📈 Real-Life Examples:
- Heights of people
- Exam scores
- Blood pressure
- Sensor errors in machines

---

## 🧠 Why It's Important:
- Foundation of **Hypothesis Testing**
- Used in **Confidence Intervals**
- Assumption in many **Machine Learning models** (like Linear Regression, Naive Bayes)

---

## ✅ Pro Tip:
Use **Z-score** to find probabilities from the Z-table or via:

```python
from scipy.stats import norm
norm.cdf(z)  # for left-tail

---
@rohitbedse_