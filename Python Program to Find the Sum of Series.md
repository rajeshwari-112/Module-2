
# Python Program to Find the Sum of Series:  
**1 + x²/2 + x³/3 + … + xⁿ/n using Function**

## 🎯 Aim
To write a Python program to compute the sum of the series using a function, where the user provides values for `n` and `x`.

## 🧠 Algorithm
1. Read the values of `n` and `x` from the user.  
2. Define a function `series(n, x)` to calculate the sum.  
   - Initialize sum `s = 1`.  
   - Use a `for` loop from 2 to `n`.  
   - Add each term `pow(x, i)/i` to the sum.  
3. Return the computed sum.  
4. Round the result to 2 decimal places and display it.

## 🧾 Program
```python
n = int(input("Enter the value of n: "))
x = int(input("Enter the value of x: "))

def series(n, x):
    s = 1
    for i in range(2, n + 1):
        s += pow(x, i) / i
    return s     

res = float(series(n, x))
print("The sum of series is", round(res, 2))
```

## Output

<img width="1328" height="887" alt="image" src="https://github.com/user-attachments/assets/4a497382-ee81-4922-9592-caa38590cdf5" />


## ✅ Result
Thus, the program has been successfully executed to compute the sum of the series using a function.

