# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:
```
def fact(i):
    if i==0 or i==1:
        return 1
    else:
        return i*fact(i-1)

def sinx(x,n):
    if n==0:
        return x
    else:
        r=(-1)**n
        q=(2*n)+1
        return ((r*(x**q)/fact(q)) + sinx(x,n-1))
        
x=int(input())
n=int(input())
print(sinx(x,n))
```
## OUTPUT
<img width="565" height="243" alt="image" src="https://github.com/user-attachments/assets/719953c9-faa1-47e1-8ab9-7baa11d36029" />

## RESULT
Thus, the program is executed successfully.
