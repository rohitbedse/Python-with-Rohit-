# 🔗 Session 34: SQL Joins

## 🔍 Topic: Understanding SQL Joins

This session explores **SQL JOIN operations**, essential for combining data across multiple tables. You'll learn different types of joins, their use cases, and how to apply them in real-world datasets.

---

### 📺 Watch the Session

🎥 [YouTube Live – SQL Joins](https://www.youtube.com/live/s6xAVqYdmJ4?si=ZF6ssuniF91ZiMFm)

---

### 📂 Resources

* 📁 [Dataset Folder (Google Drive)](https://drive.google.com/drive/folders/1RAo7rKbbnzt5Zrek1sq1pb3OJ7-IbQ5f)
* 📄 [Join Notes (PDF)](https://drive.google.com/file/d/1rHTS-h72WRcjforEcQvuK1m0ibeWG6CD/view?usp=sharing)
* 🎞️ [Interactive Join Animation – InfyTQ](https://infytq.onwingspan.com/web/en/app/toc/lex_auth_01275806667282022456_shared/overview)

---

### 🔧 Types of SQL Joins Covered

| Join Type    | Description                                            |
| ------------ | ------------------------------------------------------ |
| `INNER JOIN` | Returns matching rows from both tables                 |
| `LEFT JOIN`  | Returns all rows from the left table + matches         |
| `RIGHT JOIN` | Returns all rows from the right table + matches        |
| `FULL JOIN`  | Returns all rows when there is a match in either table |
| `SELF JOIN`  | Joins a table with itself                              |
| `CROSS JOIN` | Returns cartesian product of both tables               |

---

### 🧱 Sample Tables

#### Students

| student\_id | name    | class\_id |
| ----------- | ------- | --------- |
| 1           | Alice   | 101       |
| 2           | Bob     | 102       |
| 3           | Charlie | 103       |
| 4           | David   | NULL      |

#### Classes

| class\_id | class\_name |
| --------- | ----------- |
| 101       | Math        |
| 102       | Science     |
| 104       | History     |

---

### 🔗 Examples for Each Join Type

#### 1. INNER JOIN

Returns only rows with matching keys in both tables.

```sql
SELECT s.name, c.class_name
FROM Students s
INNER JOIN Classes c
ON s.class_id = c.class_id;
```

**Result:**

| name  | class\_name |
| ----- | ----------- |
| Alice | Math        |
| Bob   | Science     |

---

#### 2. LEFT JOIN

Returns all rows from left table and matched rows from right table, NULL if no match.

```sql
SELECT s.name, c.class_name
FROM Students s
LEFT JOIN Classes c
ON s.class_id = c.class_id;
```

**Result:**

| name    | class\_name |
| ------- | ----------- |
| Alice   | Math        |
| Bob     | Science     |
| Charlie | NULL        |
| David   | NULL        |

---

#### 3. RIGHT JOIN

Returns all rows from right table and matched rows from left table, NULL if no match.

```sql
SELECT s.name, c.class_name
FROM Students s
RIGHT JOIN Classes c
ON s.class_id = c.class_id;
```

**Result:**

| name  | class\_name |
| ----- | ----------- |
| Alice | Math        |
| Bob   | Science     |
| NULL  | History     |

---

#### 4. FULL JOIN

Returns all rows from both tables, NULL where no match.

```sql
SELECT s.name, c.class_name
FROM Students s
FULL JOIN Classes c
ON s.class_id = c.class_id;
```

**Result:**

| name    | class\_name |
| ------- | ----------- |
| Alice   | Math        |
| Bob     | Science     |
| Charlie | NULL        |
| David   | NULL        |
| NULL    | History     |

---

#### 5. SELF JOIN

Join a table to itself (example: find pairs of students in the same class).

```sql
SELECT a.name AS student1, b.name AS student2, a.class_id
FROM Students a
INNER JOIN Students b
ON a.class_id = b.class_id AND a.student_id <> b.student_id;
```

**Result:** (assuming only students in same class pairs)

| student1                                                     | student2 | class\_id |
| ------------------------------------------------------------ | -------- | --------- |
| (No matching pairs in sample data, but this is how it works) |          |           |

---

#### 6. CROSS JOIN

Cartesian product of both tables (all combinations).

```sql
SELECT s.name, c.class_name
FROM Students s
CROSS JOIN Classes c;
```

**Result:** (all student × class combinations)

| name    | class\_name |
| ------- | ----------- |
| Alice   | Math        |
| Alice   | Science     |
| Alice   | History     |
| Bob     | Math        |
| Bob     | Science     |
| Bob     | History     |
| Charlie | Math        |
| Charlie | Science     |
| Charlie | History     |
| David   | Math        |
| David   | Science     |
| David   | History     |

---

### ✅ Tips

* Use **aliases** (`s`, `c`) for readability.
* Always check for **NULL values** especially with `LEFT`, `RIGHT`, and `FULL JOIN`.
* Use `SELF JOIN` for hierarchical or comparative queries within the same table.

---

@rohitbedse_

---
