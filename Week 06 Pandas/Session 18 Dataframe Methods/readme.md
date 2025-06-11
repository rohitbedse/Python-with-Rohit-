# 🐼 Session 18: DataFrame Methods in Pandas

🎥 **Watch the full session here**: [YouTube - DataFrame Methods](https://www.youtube.com/live/zTa4MIrGTIE?si=gKobqsOzT5CxP8Ub)

This repository contains a Jupyter Notebook that demonstrates useful **DataFrame methods in Pandas** for data cleaning, transformation, and basic analysis — essential for real-world data science tasks.

## 📘 Notebook Summary

This session continues the Pandas series and focuses on **practical DataFrame methods** that make your data manipulation process faster, cleaner, and more Pythonic.

## 🧠 Key Concepts Covered

```python
# ✅ Head & Tail
df.head()         # View top 5 rows
df.tail(3)        # View last 3 rows

# ✅ Shape and Size
df.shape          # (rows, columns)
df.size           # Total number of elements

# ✅ Columns and Index
df.columns        # List of column names
df.index          # Range of index

# ✅ Data Types
df.dtypes         # Data types of each column

# ✅ Sorting
df.sort_values('column_name')               # Sort by column
df.sort_values(['col1', 'col2'], ascending=[True, False])

# ✅ Aggregations
df.sum()           # Sum of each column
df.mean()          # Column-wise mean
df['col'].value_counts()   # Frequency count

# ✅ Apply Functions
df['col'].apply(len)                 # Apply function to column
df.apply(lambda row: row.sum(), axis=1)  # Row-wise sum

# ✅ Rename Columns
df.rename(columns={'old': 'new'}, inplace=True)

# ✅ Replace Values
df.replace('old', 'new', inplace=True)

# ✅ Drop Columns / Rows
df.drop('col_name', axis=1)         # Drop column
df.drop([0, 1], axis=0)             # Drop rows by index

# ✅ Reset & Set Index
df.reset_index(drop=True, inplace=True)
df.set_index('column_name', inplace=True)
