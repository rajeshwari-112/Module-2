

# Python Program to Display Floyd's Triangle

## 🎯 Aim
To write a Python program to display Floyd's Triangle for a given number of rows.

## 🧠 Algorithm
1. Read the number of rows `n` from the user.  
2. Initialize a counter variable `k = 1`.  
3. Use a nested loop:  
   - Outer loop runs from 1 to `n` (for each row).  
   - Inner loop runs for the number of elements in that row.  
   - Print the current value of `k` and increment it.  
4. Move to the next line after each row.  

## 🧾 Program
```python
n = int(input("Enter the number of rows: "))
k = 1
for i in range(1, n + 1):
    for j in range(i):
        print("{} ".format(k), end="")
        k += 1
    print()
```

## Output

<img width="1544" height="872" alt="image" src="https://github.com/user-attachments/assets/4dfc3319-6092-47a1-b782-ceb54bae64f4" />


## ✅ Result
Thus, the program has been successfully executed to display Floyd's Triangle for the given number of rows.

