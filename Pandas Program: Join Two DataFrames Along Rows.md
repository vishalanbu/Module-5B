# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

```python
import pandas as pd

student_data1 = {
    'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'],
    'name': ['Danni', 'Ravi', 'Alex', 'Kumar', 'John'],
    'marks': [85, 90, 78, 88, 92]
}

student_data2 = {
    'student_id': ['S6', 'S7', 'S8', 'S9', 'S10'],
    'name': ['Sara', 'David', 'Priya', 'Mike', 'Anu'],
    'marks': [80, 75, 89, 91, 86]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

new_df = pd.concat([df1, df2], axis=0, ignore_index=True)

print(new_df)
```

## OUTPUT

```text
  student_id   name  marks
0         S1  Danni     85
1         S2   Ravi     90
2         S3   Alex     78
3         S4  Kumar     88
4         S5   John     92
5         S6   Sara     80
6         S7  David     75
7         S8  Priya     89
8         S9   Mike     91
9        S10    Anu     86
```

## RESULT

Thus, the two DataFrames were successfully joined row-wise using Pandas `concat()` and the combined data was stored in a new DataFrame.
