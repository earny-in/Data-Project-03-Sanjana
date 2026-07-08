# 📘 Important Pandas Commands with Explanation

## 1. import pandas as pd

### Explanation
Pandas library ko import karne ke liye use kiya jata hai.

```python
import pandas as pd
```

- `pandas` = Library ka naam
- `pd` = Alias (short name)

---

## 2. read_csv()

### Explanation
CSV file ko Python me DataFrame ke form me load karta hai.

### Syntax

```python
pd.read_csv("filename.csv")
```

### Example

```python
df = pd.read_csv("students.csv")
```

---

## 3. read_excel()

### Explanation
Excel (.xlsx) file ko read karta hai.

```python
df = pd.read_excel("students.xlsx")
```

---

## 4. head()

### Explanation
Dataset ki starting ki rows dikhata hai.

Default = First 5 Rows

```python
df.head()
```

Specific rows

```python
df.head(10)
```

---

## 5. tail()

### Explanation
Dataset ki last rows dikhata hai.

```python
df.tail()
```

---

## 6. shape

### Explanation
Rows aur Columns ki total number batata hai.

```python
df.shape
```

Output

```
(100,5)
```

Meaning

- 100 Rows
- 5 Columns

---

## 7. columns

### Explanation
Dataset ke saare column names dikhata hai.

```python
df.columns
```

Output

```
Name
Age
Marks
Gender
```

---

## 8. dtypes

### Explanation
Har column ka data type batata hai.

```python
df.dtypes
```

Example

```
Name      object
Age       int64
Marks     float64
```

---

## 9. info()

### Explanation
Dataset ki complete information deta hai.

```python
df.info()
```

Ye batata hai

- Number of rows
- Number of columns
- Missing values
- Data types
- Memory usage

---

## 10. describe()

### Explanation
Numerical columns ka statistical summary deta hai.

```python
df.describe()
```

Isme milta hai

- Count
- Mean
- Standard Deviation
- Minimum
- Maximum
- 25%
- 50%
- 75%

---

## 11. iloc[]

### Explanation
Index number ki help se data select karta hai.

```python
df.iloc[0]
```

First row

```python
df.iloc[0:5]
```

First 5 rows

---

## 12. loc[]

### Explanation
Label (row name ya index label) ke basis par data select karta hai.

```python
df.loc[0]
```

Ya

```python
df.loc[0,"Name"]
```

---

## 13. Filtering

### Explanation
Condition ke basis par data select karta hai.

```python
df[df["Marks"]>80]
```

Sirf 80 se upar marks wale students dikhenge.

---

## 14. sort_values()

### Explanation
Data ko ascending ya descending order me arrange karta hai.

Ascending

```python
df.sort_values("Marks")
```

Descending

```python
df.sort_values("Marks",ascending=False)
```

---

## 15. isnull()

### Explanation
Check karta hai kis cell me missing value hai.

```python
df.isnull()
```

---

## 16. isnull().sum()

### Explanation
Har column me kitni missing values hain, unka total count batata hai.

```python
df.isnull().sum()
```

---

## 17. fillna()

### Explanation
Missing values ko kisi value se replace karta hai.

```python
df.fillna(0)
```

Ya Mean se

```python
df.fillna(df.mean(numeric_only=True))
```

---

## 18. dropna()

### Explanation
Jis row me missing value hoti hai us row ko remove kar deta hai.

```python
df.dropna()
```

---

## 19. duplicated()

### Explanation
Duplicate rows check karta hai.

```python
df.duplicated()
```

---

## 20. drop_duplicates()

### Explanation
Duplicate rows delete karta hai.

```python
df.drop_duplicates()
```

---

## 21. mean()

### Explanation
Average value nikalta hai.

```python
df["Marks"].mean()
```

---

## 22. max()

### Explanation
Highest value batata hai.

```python
df["Marks"].max()
```

---

## 23. min()

### Explanation
Lowest value batata hai.

```python
df["Marks"].min()
```

---

## 24. sum()

### Explanation
Saare values ka total nikalta hai.

```python
df["Marks"].sum()
```

---

## 25. count()

### Explanation
Total non-null values count karta hai.

```python
df["Marks"].count()
```

---

## 26. value_counts()

### Explanation
Har unique value kitni baar aayi hai, uska count batata hai.

```python
df["Gender"].value_counts()
```

Output

```
Male      40
Female    60
```

---

## 27. unique()

### Explanation
Column ki unique values dikhata hai.

```python
df["Gender"].unique()
```

Output

```
Male
Female
```

---

## 28. groupby()

### Explanation
Same category wale data ko group karke analysis karta hai.

Example

```python
df.groupby("Gender")["Marks"].mean()
```

Male aur Female dono ka average marks alag-alag batayega.

---

## 29. merge()

### Explanation
Do DataFrames ko common column ke basis par join karta hai.

```python
pd.merge(df1,df2,on="ID")
```

---

## 30. concat()

### Explanation
Do ya usse zyada DataFrames ko ek saath jodta hai.

```python
pd.concat([df1,df2])
```

---

## 31. apply()

### Explanation
Har value par ek function apply karta hai.

```python
df["Marks"]=df["Marks"].apply(lambda x:x+5)
```

Sab students ke marks me 5 add ho jayenge.

---

## 32. to_csv()

### Explanation
DataFrame ko CSV file me save karta hai.

```python
df.to_csv("students.csv",index=False)
```

---

## 33. to_excel()

### Explanation
DataFrame ko Excel file me save karta hai.

```python
df.to_excel("students.xlsx",index=False)
```

---