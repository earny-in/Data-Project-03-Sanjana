# NumPy Library

## Introduction

NumPy (Numerical Python) is an open-source Python library used for numerical and scientific computing. It provides support for large multidimensional arrays and matrices, along with a collection of mathematical functions to operate on them efficiently.

NumPy is faster and more memory-efficient than Python lists, making it one of the most widely used libraries in Data Science, Machine Learning, and Artificial Intelligence.

---

## Installation

Install NumPy using pip:

```bash
pip install numpy
```

---

## Import NumPy

```python
import numpy as np
```

Here, `np` is an alias for NumPy.

---

# Creating Arrays

## 1D Array

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
```

Output:

```text
[1 2 3 4 5]
```

---

## 2D Array

```python
arr = np.array([
    [1, 2, 3],
    [4, 5, 6]
])

print(arr)
```

Output:

```text
[[1 2 3]
 [4 5 6]]
```

---

## 3D Array

```python
arr = np.array([
    [[1, 2], [3, 4]],
    [[5, 6], [7, 8]]
])

print(arr)
```

---

# Array Attributes

## Shape

Returns the dimensions of the array.

```python
arr.shape
```

Example output:

```text
(2, 3)
```

---

## Size

Returns the total number of elements.

```python
arr.size
```

---

## Data Type

Returns the data type of the array.

```python
arr.dtype
```

---

## Number of Dimensions

```python
arr.ndim
```

---

# Special Arrays

## Array of Zeros

```python
np.zeros((2, 3))
```

---

## Array of Ones

```python
np.ones((2, 3))
```

---

## Identity Matrix

```python
np.eye(3)
```

---

## Range of Numbers

```python
np.arange(0, 10, 2)
```

Output:

```text
[0 2 4 6 8]
```

---

## Evenly Spaced Numbers

```python
np.linspace(0, 10, 5)
```

Output:

```text
[0.0 2.5 5.0 7.5 10.0]
```

---

# Indexing and Slicing

## Access an Element

```python
arr = np.array([10, 20, 30, 40])

print(arr[0])
```

Output:

```text
10
```

---

## Slicing

```python
print(arr[1:4])
```

Output:

```text
[20 30 40]
```

---

# Reshaping Arrays

```python
arr = np.array([1, 2, 3, 4, 5, 6])

new_arr = arr.reshape(2, 3)

print(new_arr)
```

Output:

```text
[[1 2 3]
 [4 5 6]]
```

---

# Mathematical Operations

```python
a = np.array([1, 2, 3])

b = np.array([4, 5, 6])
```

## Addition

```python
a + b
```

Output:

```text
[5 7 9]
```

---

## Subtraction

```python
a - b
```

---

## Multiplication

```python
a * b
```

---

## Division

```python
a / b
```

---

# Statistical Functions

```python
arr = np.array([10, 20, 30, 40, 50])
```

## Sum

```python
np.sum(arr)
```

---

## Mean

```python
np.mean(arr)
```

---

## Median

```python
np.median(arr)
```

---

## Maximum

```python
np.max(arr)
```

---

## Minimum

```python
np.min(arr)
```

---

## Standard Deviation

```python
np.std(arr)
```

---

# Joining Arrays

```python
a = np.array([1, 2])

b = np.array([3, 4])

np.concatenate((a, b))
```

Output:

```text
[1 2 3 4]
```

---

# Splitting Arrays

```python
arr = np.array([1, 2, 3, 4, 5, 6])

np.array_split(arr, 3)
```

---

# Sorting Arrays

```python
arr = np.array([8, 3, 5, 1])

print(np.sort(arr))
```

Output:

```text
[1 3 5 8]
```

---

# Searching Arrays

```python
arr = np.array([10, 20, 30, 40])

index = np.where(arr == 30)

print(index)
```

Output:

```text
(array([2]),)
```

---

# Filtering Arrays

```python
arr = np.array([1, 2, 3, 4, 5, 6])

new_arr = arr[arr % 2 == 0]

print(new_arr)
```

Output:

```text
[2 4 6]
```

---

# Random Numbers

## Random Integer

```python
np.random.randint(1, 100)
```

---

## Random Float

```python
np.random.rand()
```

---

## Random Array

```python
np.random.rand(2, 3)
```

---

# Matrix Operations

## Matrix Multiplication

```python
a = np.array([
    [1, 2],
    [3, 4]
])

b = np.array([
    [5, 6],
    [7, 8]
])

print(np.dot(a, b))
```

---

## Transpose Matrix

```python
print(a.T)
```

---

# Copy vs View

## Copy

```python
new_arr = arr.copy()
```

Changes in the original array do not affect the copied array.

---

## View

```python
new_arr = arr.view()
```

Changes in the original array affect the view.

---

# Broadcasting

```python
arr = np.array([1, 2, 3, 4])

print(arr + 10)
```

Output:

```text
[11 12 13 14]
```

---

# Save and Load Arrays

## Save

```python
np.save("data.npy", arr)
```

## Load

```python
arr = np.load("data.npy")
```

---

# Applications of NumPy

* Data Science
* Machine Learning
* Artificial Intelligence
* Deep Learning
* Data Analysis
* Scientific Computing
* Image Processing
* Financial Analysis

---

# Advantages of NumPy

* Faster than Python lists.
* Uses less memory.
* Supports multidimensional arrays.
* Provides powerful mathematical functions.
* Easy to learn and use.

---

# Conclusion

NumPy is one of the most important Python libraries for numerical computing. It helps developers perform mathematical operations efficiently and is widely used in modern technologies such as Data Science, Artificial Intelligence, and Machine Learning.
