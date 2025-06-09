# 📊 Session 33: SQL Grouping & Sorting

## 🔍 Topic: Aggregation with `GROUP BY` & `ORDER BY`

This session explains how to **group data**, apply **aggregate functions** (like `COUNT()`, `SUM()`, `AVG()`), and sort results using `ORDER BY`. It also demonstrates combining filtering with `WHERE` and `HAVING`.

---

### 📺 Watch the Session

🔗 [YouTube Live – Session 33](https://www.youtube.com/live/nsKcmOly0UY?si=LpjUB1HJOKmWmtSS)

---

### 📂 Dataset

📄 [Download Dataset (Google Drive)](https://drive.google.com/file/d/1FQ_rZm_fvak-rVd85jlWLe1XFT_BpcMZ/view)

---

### 🧠 Key Concepts

| Clause     | Purpose                                             |
| ---------- | --------------------------------------------------- |
| `GROUP BY` | Group rows by one or more columns                   |
| `ORDER BY` | Sort result set (default ASC, use `DESC` if needed) |
| `HAVING`   | Filter grouped data (used with aggregate functions) |

---

### 📌 Example Queries

```sql
-- Group and count employees in each department
SELECT department, COUNT(*) 
FROM employees 
GROUP BY department;

-- Sort departments by total salary (descending)
SELECT department, SUM(salary) AS total_salary 
FROM employees 
GROUP BY department 
ORDER BY total_salary DESC;

-- Filter groups with average salary above 50000
SELECT department, AVG(salary) AS avg_salary 
FROM employees 
GROUP BY department 
HAVING AVG(salary) > 50000;
```

---

### ✅ Tip

Always use `HAVING` for filtering aggregated results — not `WHERE`.

---

@rohitbedse

---
