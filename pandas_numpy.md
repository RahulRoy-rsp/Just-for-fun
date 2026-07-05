# Pandas & NumPy MCQs (Medium–Intermediate) 

### 1. Which of the following is the primary difference between a NumPy array and a Python list?

A. NumPy arrays can store multiple data types in the same array.

B. NumPy arrays are optimized for numerical computations and support vectorized operations.

C. Python lists require all elements to have the same data type.

D. Python lists consume less memory in all cases.

---

### 2. Which Pandas data structure is best suited for representing tabular data with labeled rows and columns?

A. ndarray

B. Series

C. DataFrame

D. Dictionary

---

### 3. What is the primary purpose of the `axis` parameter in many Pandas functions?

A. To specify the data type

B. To indicate whether the operation is row-wise or column-wise

C. To sort the data

D. To remove duplicate values

---

### 4. Which NumPy function creates an array with evenly spaced values over a specified interval?

A. `zeros()`

B. `linspace()`

C. `reshape()`

D. `append()`

---

### 5. Which Pandas function is commonly used to combine two DataFrames based on one or more common columns?

A. `concat()`

B. `merge()`

C. `append()`

D. `join_axes()`

---

### 6. What is the primary advantage of vectorized operations in NumPy?

A. They reduce memory usage by compressing arrays.

B. They eliminate the need for loops, improving performance.

C. They automatically sort the data.

D. They prevent missing values.

---

### 7. In Pandas, what does the `iloc[]` indexer use for selection?

A. Column names

B. Boolean conditions

C. Integer-based positions

D. Index labels

---

### 8. Which statement about a Pandas `Series` is correct?

A. It always contains multiple columns.

B. It is a one-dimensional labeled array.

C. It cannot store string values.

D. It always uses integer indexing.

---

### 9. What is the purpose of the `groupby()` function in Pandas?

A. To sort rows alphabetically

B. To split data into groups for aggregation or analysis

C. To remove duplicate rows

D. To combine multiple DataFrames

---

### 10. Which NumPy function returns the dimensions of an array?

A. `shape`

B. `dtype`

C. `size`

D. `ndim`

---

### 11. Which Pandas function is commonly used to identify missing values?

A. `dropna()`

B. `fillna()`

C. `isna()`

D. `replace()`

---

### 12. Which operation is commonly referred to as **broadcasting** in NumPy?

A. Copying arrays between variables

B. Automatically expanding arrays of compatible shapes during arithmetic operations

C. Combining multiple arrays into one

D. Sorting multidimensional arrays

---

### 13. Which of the following best describes a NumPy ndarray?

A. A mutable, multidimensional array with homogeneous data type

B. A collection of heterogeneous Python objects

C. A two-dimensional table with labeled columns

D. A dictionary-like structure

---

### 14. Which Pandas method removes rows containing missing values?

A. `fillna()`

B. `dropna()`

C. `replace()`

D. `drop_duplicates()`

---

### 15. Which attribute returns the total number of elements in a NumPy array?

A. `shape`

B. `size`

C. `dtype`

D. `ndim`

---

### 16. Which function is commonly used to read a CSV file into a Pandas DataFrame?

A. `read_table()`

B. `read_excel()`

C. `read_csv()`

D. `load_csv()`

---

### 17. Which Pandas method is primarily used to sort a DataFrame based on column values?

A. `sort()`

B. `order()`

C. `sort_values()`

D. `arrange()`

---

### 18. Which NumPy function creates an identity matrix?

A. `ones()`

B. `diag()`

C. `eye()`

D. `identity_matrix()`

---

### 19. What is the purpose of the `describe()` method in Pandas?

A. To rename columns

B. To display summary statistics of numerical data

C. To remove duplicate rows

D. To visualize the dataset

---

### 20. Which of the following best describes **boolean indexing** in Pandas?

A. Selecting rows or columns using logical conditions

B. Selecting rows by integer positions

C. Selecting columns alphabetically

D. Selecting rows randomly

---

### 21. Which NumPy attribute indicates the number of dimensions of an array?

A. `shape`

B. `size`

C. `dtype`

D. `ndim`

---

### 22. Which Pandas method removes duplicate rows from a DataFrame?

A. `dropna()`

B. `drop_duplicates()`

C. `unique()`

D. `distinct()`

---

### 23. What is the primary purpose of the `astype()` method in Pandas?

A. To rename columns

B. To change the data type of a Series or DataFrame column

C. To convert a DataFrame into a NumPy array

D. To remove invalid values

---

### 24. Which NumPy function is commonly used to compute the mean of an array?

A. `average()`

B. `mean()`

C. `median()`

D. `sum()`

---

### 25. Which Pandas function is most appropriate for combining DataFrames vertically (stacking rows)?

A. `merge()`

B. `concat()`

C. `join()`

D. `combine()`

---

### 26. Which statement about NumPy arrays is correct?

A. All elements in an array typically share the same data type.

B. Every element can have a different data type without affecting performance.

C. Arrays cannot be multidimensional.

D. Arrays cannot store floating-point values.

---

### 27. Which Pandas function is commonly used to replace missing values with a specified value?

A. `replace()`

B. `fillna()`

C. `dropna()`

D. `isna()`

---

### 28. Which of the following best describes the result of `df.head()`?

A. Returns the last five rows of a DataFrame.

B. Returns summary statistics.

C. Returns the first few rows of a DataFrame.

D. Returns only the column names.

---

### 29. Which NumPy function changes the shape of an array without changing its data?

A. `resize()`

B. `reshape()`

C. `flatten()`

D. `transpose()`

---

### 30. Which Pandas operation is most appropriate for calculating aggregate statistics (such as mean or sum) for different categories within a dataset?

A. `sort_values()`

B. `groupby()`

C. `drop_duplicates()`

D. `reset_index()`


---

### 1. In NumPy, what is a **view** compared to a **copy**?

A. A view duplicates data in memory

B. A view shares the same memory as the original array

C. A view is always immutable

D. A view is slower because it recomputes values

---

### 2. What will happen when you modify a slice of a NumPy array that is a view?

A. Original array remains unchanged

B. Only the sliced array changes independently

C. Original array is also modified

D. An error is thrown

---

### 3. Which Pandas operation is most likely to trigger **copy-on-write behavior (if enabled in modern versions)**?

A. Direct column assignment using `.loc`

B. Using `groupby()` aggregation

C. Sorting a DataFrame

D. Reading a CSV file

---

### 4. What is the main difference between `apply()` and `map()` in Pandas?

A. `apply()` works only on DataFrames, `map()` only on Series

B. `map()` works element-wise on Series, while `apply()` is more general

C. `apply()` is faster in all cases

D. `map()` works only with numeric data

---

### 5. What is a key limitation of using Python loops over NumPy operations?

A. Loops cannot handle integers

B. Loops are vectorized

C. Loops do not utilize low-level optimizations like SIMD

D. Loops automatically parallelize

---

### 6. In Pandas, what is the effect of setting `inplace=True`?

A. Creates a backup of the DataFrame

B. Modifies the original object without returning a new one

C. Improves execution speed in all cases

D. Converts the DataFrame into a Series

---

### 7. What does NumPy **broadcasting failure** typically result in?

A. Automatic reshaping of arrays

B. Silent truncation of arrays

C. A ValueError due to incompatible shapes

D. Conversion to object dtype

---

### 8. Which scenario best describes a **chained assignment problem** in Pandas?

A. Using multiple groupby operations

B. Assigning values through multiple indexing steps that may operate on a copy

C. Merging multiple DataFrames

D. Sorting after filtering

---

### 9. Why is chained indexing discouraged in Pandas?

A. It is slower than groupby

B. It always produces incorrect results

C. It may operate on a temporary copy rather than the original DataFrame

D. It is deprecated in all versions

---

### 10. Which NumPy function is most appropriate for linear algebra operations like matrix multiplication?

A. `multiply()`

B. `dot()`

C. `sum()`

D. `cross()`

---

### 11. What does `np.where(condition, x, y)` return?

A. Indices where condition is True

B. Elements from x or y based on condition

C. Only boolean values

D. Filtered array of x only

---

### 12. Which Pandas function is most suitable for reshaping data from long to wide format?

A. `melt()`

B. `pivot()`

C. `stack()`

D. `concat()`

---

### 13. What is the key difference between `pivot()` and `pivot_table()`?

A. `pivot()` handles aggregation, `pivot_table()` does not

B. `pivot_table()` supports aggregation and duplicate handling

C. `pivot()` works only on numeric data

D. There is no difference

---

### 14. What is the main risk of using `fillna(method='ffill')`?

A. It deletes rows

B. It may propagate incorrect assumptions across missing data

C. It converts data types

D. It removes duplicates

---

### 15. In NumPy, what does `axis=0` typically represent in a 2D array?

A. Row-wise operation

B. Column-wise operation

C. Entire matrix flattening

D. Diagonal operation

---

### 16. Which Pandas method is used internally for aligning data before arithmetic operations?

A. Broadcasting engine

B. Index alignment mechanism

C. Merge optimizer

D. Sort index handler

---

### 17. What happens when two Pandas Series with different indexes are added?

A. Error is thrown

B. Positional addition occurs

C. Alignment is performed based on index labels

D. Only overlapping values are dropped

---

### 18. Which NumPy function is most appropriate for generating random samples from a normal distribution?

A. `rand()`

B. `randint()`

C. `normal()`

D. `choice()`

---

### 19. What is the main advantage of using categorical data type in Pandas?

A. Faster arithmetic operations

B. Reduced memory usage for repetitive string data

C. Automatic sorting

D. Eliminates missing values

---

### 20. What is the effect of converting a Pandas column to `category` type?

A. It increases memory usage

B. It stores unique values as codes internally

C. It converts values into floats

D. It disables indexing on that column

---

---
