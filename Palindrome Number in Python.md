
# Palindrome Number in Python

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
