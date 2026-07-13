# Pandas short notes

## Introduction

Pandas is a powerful Python library used for data analysis and manipulation. It provides easy-to-use data structures and functions for working with structured data.

```python
import pandas as pd
```

---

# Reading Data

## Read a CSV file

```python
df = pd.read_csv("data.csv")
```

**Explanation:** Loads data from a CSV file into a DataFrame.

## Read an Excel file

```python
df = pd.read_excel("data.xlsx")
```

**Explanation:** Loads data from an Excel file.

---

# Viewing Data

## Display the first five rows

```python
df.head()
```

**Explanation:** Shows the first five rows of the dataset.

## Display the last five rows

```python
df.tail()
```

**Explanation:** Shows the last five rows of the dataset.

## Get information about the dataset

```python
df.info()
```

**Explanation:** Displays column names, data types, and missing values.

## Generate statistical summary

```python
df.describe()
```

**Explanation:** Provides statistical information such as mean, minimum, maximum, and standard deviation.

---

# Dataset Information

## Get the shape of the dataset

```python
df.shape
```

**Explanation:** Returns the number of rows and columns.

## Display column names

```python
df.columns
```

**Explanation:** Returns all column names.

## Display data types

```python
df.dtypes
```

**Explanation:** Shows the data type of each column.

---

# Selecting Data

## Select a single column

```python
df["Name"]
```

**Explanation:** Selects the "Name" column.

## Select multiple columns

```python
df[["Name", "Age"]]
```

**Explanation:** Selects multiple columns from the DataFrame.

## Select rows using index

```python
df.iloc[0]
```

**Explanation:** Selects the first row using its index position.

## Select rows using labels

```python
df.loc[0]
```

**Explanation:** Selects rows using labels.

---

# Filtering Data

## Filter rows based on a condition

```python
df[df["Age"] > 18]
```

**Explanation:** Returns rows where the age is greater than 18.

---

# Handling Missing Values

## Check missing values

```python
df.isnull()
```

**Explanation:** Identifies missing values in the dataset.

## Count missing values

```python
df.isnull().sum()
```

**Explanation:** Counts the number of missing values in each column.

## Remove missing values

```python
df.dropna()
```

**Explanation:** Removes rows containing missing values.

## Fill missing values

```python
df.fillna(0)
```

**Explanation:** Replaces missing values with a specified value.

---

# Sorting Data

## Sort values in ascending order

```python
df.sort_values("Age")
```

**Explanation:** Sorts the dataset based on the "Age" column.

## Sort values in descending order

```python
df.sort_values("Age", ascending=False)
```

**Explanation:** Sorts the dataset in descending order.

---

# Grouping Data

## Group data by a column

```python
df.groupby("Department").mean()
```

**Explanation:** Groups the data and calculates the average values.

---

# Modifying Data

## Add a new column

```python
df["Salary"] = [30000, 40000, 50000]
```

**Explanation:** Adds a new column to the DataFrame.

## Remove a column

```python
df.drop("Salary", axis=1)
```

**Explanation:** Deletes a column from the DataFrame.

## Rename columns

```python
df.rename(columns={"Name": "Full_Name"})
```

**Explanation:** Changes the name of a column.

---

# Removing Duplicates

## Remove duplicate rows

```python
df.drop_duplicates()
```

**Explanation:** Deletes duplicate rows from the dataset.

---

# Combining DataFrames

## Merge two DataFrames

```python
pd.merge(df1, df2, on="ID")
```

**Explanation:** Combines two DataFrames using a common column.

## Concatenate DataFrames

```python
pd.concat([df1, df2])
```

**Explanation:** Joins multiple DataFrames together.

---

# Working with Unique Values

## Count unique values

```python
df["City"].value_counts()
```

**Explanation:** Counts the occurrence of each unique value.

## Get unique values

```python
df["City"].unique()
```

**Explanation:** Returns all unique values from a column.

## Count the number of unique values

```python
df["City"].nunique()
```

**Explanation:** Returns the total number of unique values.

---

# Changing Data Types

## Convert data type

```python
df["Age"] = df["Age"].astype(int)
```

**Explanation:** Converts the data type of a column.

---

# Creating a Copy

## Create a copy of the DataFrame

```python
new_df = df.copy()
```

**Explanation:** Creates a duplicate copy of the DataFrame.

---

# Saving Data

## Save as CSV

```python
df.to_csv("output.csv")
```

**Explanation:** Saves the DataFrame as a CSV file.

## Save as Excel

```python
df.to_excel("output.xlsx")
```

**Explanation:** Saves the DataFrame as an Excel file.

---

# Conclusion

Pandas provides powerful functions for reading, analyzing, cleaning, and manipulating data. These commands are the most important and commonly used functions in data analysis and machine learning projects.