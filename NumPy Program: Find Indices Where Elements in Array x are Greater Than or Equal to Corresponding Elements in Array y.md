# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program

```python id="t3k7qm"
import numpy as np

x = np.array([10, 20, 30, 40, 50])
y = np.array([5, 25, 30, 45, 40])

indices = np.where(x >= y)

print("Indices where x is greater than or equal to y:")
print(indices[0])
```

## Output

```text id="n5p8rx"
Indices where x is greater than or equal to y:
[0 2 4]
```


## Result
Thus, the NumPy program successfully finds and displays the indices where the elements of array `x` are greater than or equal to the corresponding elements of array `y`.
