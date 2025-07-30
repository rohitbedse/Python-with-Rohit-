# 📊 Session 45 – Hypothesis Testing

## 🔍 What You Learned:
**Hypothesis Testing** is a statistical method to test assumptions (claims) about a population using sample data.

---

## 🧠 Core Concepts:

| Term                | Meaning |
|---------------------|---------|
| **Null Hypothesis (H₀)**     | No effect / No difference claim (status quo) |
| **Alternative Hypothesis (H₁)** | What we want to prove (change exists) |
| **p-value**         | Probability that results occurred by chance |
| **Significance Level (α)** | Threshold to reject H₀ (commonly 0.05) |

---

## ✅ Decision Rule:

- If **p-value < α**, reject H₀ → evidence supports H₁  
- If **p-value ≥ α**, **fail to reject H₀** → not enough evidence

---

## 📌 Types of Hypothesis Tests:

| Test Type     | Use Case                      |
|---------------|-------------------------------|
| One-tailed    | Directional test (greater/less) |
| Two-tailed    | Non-directional (difference only) |

---

## 🔁 Errors in Hypothesis Testing:

| Type           | Meaning                         |
|----------------|---------------------------------|
| **Type I Error** | Rejecting H₀ when it's true (false alarm) |
| **Type II Error**| Failing to reject H₀ when it's false (missed detection) |

---

## 🛠️ Resources Used:

- 📺 [YouTube Session](https://www.youtube.com/live/S94mx6OL7kM?si=vJfh_PMVmsMse4lG)
- 📘 [PDF Notes](https://drive.google.com/file/d/1J6TWERqWu1-98n2b8uBKdU8j0aCVgyuN/view)

---

## 📈 Real-Life Examples:

- Does a new drug work better than the old one?  
- Is the average salary different this year?  
- Is a new teaching method more effective?

---

## ✅ Pro Tip (Python):

```python
from scipy import stats

# Example: One sample t-test
sample = [sample_data]
t_stat, p_val = stats.ttest_1samp(sample, popmean=known_value)

if p_val < 0.05:
    print("Reject Null Hypothesis")
else:
    print("Fail to Reject Null Hypothesis")

@rohitbedse_