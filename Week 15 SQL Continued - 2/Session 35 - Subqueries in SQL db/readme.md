# 🎯 Session 35: Subqueries in SQL

## 📚 Topic Overview

This session covers **subqueries** in SQL — queries nested inside other queries. You’ll learn how to use subqueries in SELECT, WHERE, and FROM clauses to write more powerful and flexible SQL statements.

---

### 🎥 Watch the Session

[YouTube Live – Subqueries in SQL](https://www.youtube.com/live/YYq47MN3TZI?si=EJlk_sqQI0tdXeFd)

---

### 📂 Resources

* 📁 [Dataset Folder (Google Drive)](https://drive.google.com/drive/folders/1xCNbO_LJIkr7bi9YDa7hUFYgJ-IZ01A-?usp=share_link)
* 📄 [Session Notes (PDF)](https://drive.google.com/file/d/1sV47jQOTJGo9ZltUP6nwcKGBMF1rbmK9/view?usp=drive_link)

---

### 🐍 Python tip: Reading movies.csv file

```python
import pandas as pd

df = pd.read_csv('movies.csv', delimiter=';', encoding_errors='ignore')
```

* Use `delimiter=';'` because the CSV file uses semicolon as separator.
* `encoding_errors='ignore'` to avoid errors from bad characters in the file.

---

### 💡 Quick Subquery Example

```sql
-- Find movies with rating above average rating
SELECT movie_title, rating
FROM Movies
WHERE rating > (
    SELECT AVG(rating) FROM Movies
);
```

---

@rohitbedse_

---
