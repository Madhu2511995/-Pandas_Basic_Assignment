# Pandas_Basic_Assignment
Title: DataFrames and Series in Pandas: Building Blocks of Data Manipulation

Introduction:
Pandas is a popular Python library that provides powerful tools for data manipulation and analysis. At the heart of Pandas lie two fundamental data structures: DataFrames and Series. Understanding these structures is essential for effectively working with tabular data in Python. This article aims to explain DataFrames and Series, their characteristics, and some common functions that make data manipulation a breeze.

1. Series - The Building Block:
A Series is a one-dimensional labeled array-like object provided by Pandas. It is similar to a NumPy array, but with an index attached to each element. The index serves as a unique label for each data point, enabling efficient data alignment and easier access to elements.

Creating a Series:
```python
import pandas as pd

data = [10, 20, 30, 40, 50]
index = ['A', 'B', 'C', 'D', 'E']
series = pd.Series(data, index=index)
print(series)
```

Output:
```
A    10
B    20
C    30
D    40
E    50
dtype: int64
```

2. DataFrames - Tabular Data at its Finest:
A DataFrame is a two-dimensional data structure that resembles a table or spreadsheet. It is a collection of Series where each Series represents a column of the DataFrame. This tabular structure with labeled rows and columns allows for seamless manipulation of structured data.

Creating a DataFrame:
```python
data = {
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [25, 30, 22, 28],
    'City': ['New York', 'London', 'Paris', 'Tokyo']
}

df = pd.DataFrame(data)
print(df)
```

Output:
```
      Name  Age      City
0    Alice   25  New York
1      Bob   30    London
2  Charlie   22     Paris
3    David   28     Tokyo
```

3. Common Functions for Data Manipulation:

a) DataFrame Functions:
- `df.head(n)`: Returns the first 'n' rows of the DataFrame.
- `df.tail(n)`: Returns the last 'n' rows of the DataFrame.
- `df.info()`: Provides a summary of the DataFrame's structure.
- `df.describe()`: Generates descriptive statistics of the DataFrame's numerical columns.
- `df.drop(labels, axis=, inplace=)`: Drops specified rows or columns from the DataFrame.

b) Series Functions:
- `series.head(n)`: Returns the first 'n' elements of the Series.
- `series.tail(n)`: Returns the last 'n' elements of the Series.
- `series.mean()`: Calculates the mean of the elements in the Series.
- `series.unique()`: Returns an array of unique elements in the Series.
- `series.apply(func)`: Applies a function to each element of the Series.

Conclusion:
Pandas' DataFrame and Series are powerful data structures that form the backbone of data manipulation in Python. Series provides a labeled one-dimensional array, while DataFrame extends this concept into a two-dimensional tabular format. Understanding how to create, access, and manipulate Series and DataFrames, along with using common functions, is essential for any data analysis or manipulation task. With the versatility of these structures and the rich collection of functions offered by Pandas, working with structured data becomes a seamless and enjoyable experience.
