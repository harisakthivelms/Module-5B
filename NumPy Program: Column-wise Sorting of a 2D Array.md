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
import numpy as np
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))
array = []
print("Enter the elements row-wise:")
for _ in range(rows):
    row = list(map(int, input().split()))
    array.append(row)
arr = np.array(array)
sorted_arr = np.sort(arr, axis=0)
print("Original array:")
print(arr)
print("Column-wise sorted array:")
print(sorted_arr)


## Output
<img width="500" height="510" alt="image" src="https://github.com/user-attachments/assets/f0cb152f-b599-4a46-814d-ae86fedf07bb" />

## Result
thus the code excuted sucessfully
