# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```python id="v6m2kp"
import numpy as np

a = np.array([[1, 2, 3],
              [4, 5, 6],
              [7, 8, 9]])

new_column = np.array([10, 20, 30])

a = np.delete(a, 1, axis=1)
a = np.insert(a, 1, new_column, axis=1)

print("Updated Array:")
print(a)
```

## Output

```text id="k3r8qn"
Updated Array:
[[ 1 10  3]
 [ 4 20  6]
 [ 7 30  9]]
```

## Result

Thus, the NumPy program successfully replaces the second column of the given 2D array with a new column.
