# 🔁 Recursion:Palindrome Checker Using Recursion in Python

## 🎯 AIM:
To write a Python program to check whether a given string is a **palindrome** using **recursion**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `is_palindrome(word)`
   - **Base Case:** If the string length is less than 1, return `True`
   - **Recursive Case:** If the first and last characters match, call the function recursively on the substring without first and last characters
   - Else, return `False`
3. Get input from the user
4. Call the recursive function
5. Print whether the string is a palindrome
6. **Stop**

---

## 💻 PROGRAM:
```
def is_palindrome(word):
    # Base case
    if len(word) < 1:
        return True
    
    # Recursive case
    if word[0] == word[-1]:
        return is_palindrome(word[1:-1])
    else:
        return False

s = input("Enter a word: ")

if is_palindrome(s):
    print("String is a palindrome")
else:
    print("String is not a palindrome")

```
## OUTPUT
<img width="626" height="261" alt="image" src="https://github.com/user-attachments/assets/c39f34f7-acca-42f8-81a3-5fd3d883f7b6" />

## RESULT
Thus, the program is executed successfully.
