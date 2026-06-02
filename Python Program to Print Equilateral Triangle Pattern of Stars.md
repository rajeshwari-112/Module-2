

# Python Program to Print Equilateral Triangle Pattern of Stars

## 🎯 Aim
To write a Python program to print an equilateral triangle pattern of stars for a given number of rows.

## 🧠 Algorithm
1. Read the number of rows `n` from the user.  
2. Use a loop to iterate from 0 to `n-1` (for each row).  
3. For each row:  
   - Print leading spaces to align the stars symmetrically.  
   - Print stars separated by spaces.  
4. Move to the next line after each row.  

## 🧾 Program
```python
n = int(input("Enter the number of rows: "))

for i in range(0, n):
    # print leading spaces
    for s in range(2 * n - i - 2):
        print(" ", end="")
    # print stars
    for j in range(i + 1):
        print("*  ", end="")
    print()
```

## 🖥️ Example Output
<img width="1528" height="868" alt="image" src="https://github.com/user-attachments/assets/d47ae5ee-0b9d-4d41-a452-37be2885cb73" />



## ✅ Result
Thus, the program has been successfully executed to print an equilateral triangle star pattern for the given number of rows.

