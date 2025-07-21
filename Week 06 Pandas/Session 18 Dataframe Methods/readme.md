# 🐼 Session 18: DataFrame Methods in Pandas

🎥 **Watch the full session here**: [YouTube - DataFrame Methods](https://www.youtube.com/live/zTa4MIrGTIE?si=gKobqsOzT5CxP8Ub)

This repository contains a Jupyter Notebook that demonstrates useful **DataFrame methods in Pandas** for data cleaning, transformation, and basic analysis — essential for real-world data science tasks.

## 📘 Notebook Summary

This session continues the Pandas series and focuses on **practical DataFrame methods** that make your data manipulation process faster, cleaner, and more Pythonic.

## 🧠 Key Concepts Covered

---

**value_counts()** → Returns frequency counts of unique values in a Series.  
`df['col'].value_counts()`

**sort_values()** → Sorts the DataFrame by column values.  
`df.sort_values('col', ascending=False)`

**rank()** → Assigns ranks to entries in a Series or DataFrame.  
`df['col'].rank()`

**sort_index()** → Sorts the DataFrame by its index (not values).  
`df.sort_index(ascending=True)`

**set_index()** → Sets one or more columns as the index.  
`df.set_index('col', inplace=True)`

**rename()** → Renames columns or index entries.  
`df.rename(columns={'old': 'new'}, index={0: 'first'})`

**reset_index()** → Resets the index to default and moves index to a column.  
`df.reset_index(drop=True, inplace=True)`

**unique() & nunique()** → `unique()` gives unique values, `nunique()` counts them.  
`df['col'].unique()`  
`df['col'].nunique()`

**isnull() / notnull() / hasnans** → Checks for missing values.  
`df.isnull()`, `df.notnull()`, `df.hasnans`

**dropna()** → Removes rows or columns with missing values.  
`df.dropna(axis=0)`  # rows  
`df.dropna(axis=1)`  # columns

**fillna()** → Fills missing values with specified value or method.  
`df.fillna(0)`  
`df.fillna(method='ffill')`

**drop_duplicates()** → Removes duplicate rows.  
`df.drop_duplicates()`

**drop()** → Drops rows/columns by labels.  
`df.drop('col', axis=1)`  
`df.drop([0, 1], axis=0)`

**apply()** → Applies a function to each row/column.  
`df['col'].apply(lambda x: x * 2)`

**isin()** → Checks whether each element is in a given list.  
`df['col'].isin([10, 20, 30])`

**corr()** → Computes pairwise correlation between columns.  
`df.corr()`

**nlargest() / nsmallest()** → Returns rows with largest/smallest values.  
`df.nlargest(5, 'col')`  
`df.nsmallest(3, 'col')`

**insert()** → Inserts a new column at a specific position.  
`df.insert(1, 'new_col', [1,2,3])`

**copy()** → Creates a deep copy of the DataFrame.  
`df_copy = df.copy()`

---

