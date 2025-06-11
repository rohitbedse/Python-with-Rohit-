# 🐼 Session 17: Pandas DataFrames

🎥 **Watch the full session here**: [YouTube - Pandas DataFrames](https://www.youtube.com/live/OG31yhRQxPI?si=KmsTOgksO828LBMQ)

This repository contains a Jupyter Notebook that introduces and demonstrates key operations using **Pandas DataFrames**, one of the most powerful data structures for data manipulation in Python.

## 📘 Notebook Summary

The notebook is part of a structured learning path in **Data Science and Python Programming**, especially focusing on **data preprocessing and exploration** using the `pandas` library.

## 🧠 Key Concepts Covered

```python
# ✅ Creating a DataFrame
import pandas as pd
data = {'Name': ['Alice', 'Bob'], 'Marks': [85, 90]}
df = pd.DataFrame(data)

# ✅ Basic Info & Description
df.info()        # Summary of structure
df.describe()    # Statistical description

# ✅ Accessing Columns and Rows
df['Name']                # Single column
df[['Name', 'Marks']]     # Multiple columns
df.iloc[0]                # Row by index
df.loc[0]                 # Row by label

# ✅ Handling Missing and Duplicate Data
df.isnull()                    # Detect missing values
df.dropna()                    # Remove missing
df.duplicated()                # Detect duplicates
df.drop_duplicates(inplace=True)  # Remove duplicates

# ✅ Modifying the DataFrame
df['Marks'] += 5              # Update values
df.drop('Marks', axis=1)      # Drop column

# ✅ Sorting & Filtering
df.sort_values('Name')        # Sort alphabetically
df[df['Marks'] > 80]          # Conditional filtering

# ✅ Slicing and Indexing
df[:2]                # Slice first 2 rows
df.iloc[:, :1]        # Slice first column
