# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program

```python id="q7m2vx"
import numpy as np

a = np.array([[3, 2, 1],
              [6, 5, 4],
              [9, 8, 7]])

print("Original Array:")
print(a)

sorted_array = np.sort(a, axis=0)

print("Column-wise Sorted Array:")
print(sorted_array)
```

## Output
```text id="r8k4pn"
Original Array:
[[3 2 1]
 [6 5 4]
 [9 8 7]]

Column-wise Sorted Array:
[[3 2 1]
 [6 5 4]
 [9 8 7]]
```

## Result
Thus, the NumPy program successfully sorts the elements of each column of a 2D array in ascending order.
