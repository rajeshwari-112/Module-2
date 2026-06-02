
# EX:1 Palindrome Number in Python

## 🎯 Aim
To write a Python program that checks whether a given number is a palindrome.

## 🧠 Algorithm
1. Read an integer from the user using `input()`.
2. Store the original number in a variable `n`.
3. Reverse the number using a `while` loop:
   - Extract the last digit using modulus (`%`).
   - Build the reversed number by multiplying the current reversed value by 10 and adding the digit.
   - Reduce the number using integer division (`//`).
4. Compare the original number with the reversed number.
5. If both are equal, the number is a palindrome; otherwise, it is not.

## 🧾 Program
```python
n = int(input("Enter a number: "))
num = n
rev = 0

while num > 0:
    rem = num % 10
    rev = rev * 10 + rem
    num //= 10  # Use integer division

if n == rev:  # Compare the original number 'n' with the reversed number 'rev'
    print(f"The given number {n} is a Palindrome")
else:
    print(f"The given number {n} is not a Palindrome")
```

##  Output
<img width="1330" height="825" alt="image" src="https://github.com/user-attachments/assets/8f1515cc-d44d-41c0-bdc6-1987f98bcaf6" />


## ✅ Result
Thus, the program has been successfully executed to check whether a given number is a palindrome.
<br>
<br>

# EX:2 Python Program Using Lambda Function

## 🎯 Aim
To write a Python program that uses a lambda function to multiply a given number by 56.

## 🧠 Algorithm
1. Read an integer input from the user.  
2. Define a lambda function that takes a parameter `x` and returns `x * 56`.  
3. Pass the user input to the lambda function.  
4. Print the result.  

## 🧾 Program
```python
n = int(input("Enter a number: "))
square = lambda x: x * 56
print(square(n))
```

## 🖥️ Example Output

<img width="1325" height="839" alt="image" src="https://github.com/user-attachments/assets/d97f3a2f-88af-4103-8990-22be222ccc1f" />


## ✅ Result
Thus, the program has been successfully executed using a lambda function to multiply the given number by 56.


<br>
<br>


# EX:3 Python Program to Display Floyd's Triangle

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




<br>
<br>


# EX:4 Python Program to Find the Sum of Series:  
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



<br>
<br>



# EX:5 Python Program to Print Equilateral Triangle Pattern of Stars

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





