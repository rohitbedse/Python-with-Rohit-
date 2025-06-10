# 📊 Pandas Series Tutorial

This repository covers the foundational concepts and practical usage of **pandas Series** in Python for data analysis.

---

## 📅 Version Information (as of June 10, 2025)

* **Python:** 3.11+
* **pandas:** 2.2.2
* **matplotlib (optional, for plotting):** 3.9.0

To check your installed versions:

```bash
python --version
pip show pandas matplotlib
```

Install the required libraries:

```bash
pip install pandas matplotlib
```

---

## 📁 Dataset

🔗 [Google Drive - Dataset Folder](https://drive.google.com/drive/folders/1aUJ85Ea-TxVWSQNvtKjkz75fqEAqFHk6)

---

## 🎥 Video Tutorial

Watch the full tutorial here:
🔗 [YouTube Live Session](https://www.youtube.com/live/zCDVUyq8lkw?si=XD45shjQEYcOTZLp)

---

## 📘 Topics Covered

### ✅ What is pandas?

* **pandas** is a fast, flexible, and expressive data analysis library built on top of NumPy.

---

### ✅ pandas Series

* A one-dimensional labeled array capable of holding any data type.
* Similar to a column in an Excel sheet.

---

### ✅ Series Attributes

* `.index` – index labels
* `.values` – underlying NumPy array
* `.dtype` – data type
* `.size`, `.shape`, `.ndim` – size and dimensionality

---

### ✅ Creating Series

* From a list, dictionary, scalar, or NumPy array:

  ```python
  import pandas as pd
  s = pd.Series([10, 20, 30])
  ```

* From a CSV file using `read_csv()`:

  ```python
  series = pd.read_csv("file.csv").squeeze()
  ```

---

### ✅ Series Methods

* `.head()`, `.tail()`
* `.value_counts()`
* `.sort_values()`, `.sort_index()`
* `.unique()`, `.nunique()`

---

### ✅ Series Math Methods

* `.sum()`, `.mean()`, `.median()`, `.std()`, `.max()`, `.min()`
* Arithmetic operations: `series + 10`, `series ** 2`

---

### ✅ Series Indexing

* Positional indexing: `series[0]`
* Label-based indexing: `series['label']`
* Slicing: `series[1:5]`, `series['a':'d']`

---

### ✅ Editing Series

* Modify values using index
* Rename or reassign index labels
* Append or remove elements

---

### ✅ Copy and Views

* Use `.copy()` to avoid unwanted changes due to referencing
* Understand difference between view vs copy

---

### ✅ Series with Python Functionalities

* Use `map()`, `filter()`, `lambda`, and list comprehensions on Series
* Example:

  ```python
  s = pd.Series([1, 2, 3])
  s = s.map(lambda x: x * 2)
  ```

---

### ✅ Boolean Indexing on Series

* Apply conditions directly:

  ```python
  s = pd.Series([100, 200, 300])
  s[s > 150]
  ```

---

### ✅ Plotting Graphs on Series

* Basic visualization with `matplotlib` or built-in `.plot()`:

  ```python
  s.plot(kind='bar')  # bar, line, pie
  ```

---

### ✅ Some Important Series Methods

* `.isnull()`, `.notnull()`
* `.dropna()`, `.fillna()`
* `.apply()`, `.map()` for element-wise transformations

---

## 👨‍💻 Author

**Rohit Bedse**
🔗 [LinkedIn](https://www.linkedin.com/in/rohit-bedse-086b86262/)
📂 [Portfolio](https://portfolio-demo-seven-lyart.vercel.app/)

---

@rohitbedse_

---
