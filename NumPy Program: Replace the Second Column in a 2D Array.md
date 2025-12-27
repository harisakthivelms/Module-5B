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

import numpy as np


rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements of the original array row-wise:")
array = []
for _ in range(rows):
    row = list(map(int, input().split()))
    array.append(row)
arr = np.array(array)

print(f"Enter {rows} elements of the new column:")
new_col = np.array(list(map(int, input().split()))).reshape(rows, 1)

arr = np.delete(arr, 1, axis=1)

arr = np.insert(arr, 1, new_col, axis=1)

print("Updated array with replaced column:")
print(arr)


## Output
<img width="584" height="483" alt="image" src="https://github.com/user-attachments/assets/5119d035-78b3-4e6b-938c-cb656451d5b3" />

## Result
thus code excuted sucessfully
