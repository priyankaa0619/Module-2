# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```
a = 16
binary_value = bin(a)
print("Binary representation of", a, "is:", binary_value)
```

## Output

<img width="482" height="194" alt="image" src="https://github.com/user-attachments/assets/831cc3ca-ee6b-4465-ac8b-9625b5238b0e" />


## Result
The program successfully converts the number 16 into its binary representation using the built-in bin() function in Python.
# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
```
def result(a, b):
    mod = a % b
    print("Modulo is:", mod)


a = int(input("Enter first number: "))
b = int(input("Enter second number: "))


result(a, b)
```


## Output

<img width="436" height="261" alt="image" src="https://github.com/user-attachments/assets/f4a4325e-e3f7-408c-8d9c-87cc59547276" />


## Result
The program successfully defines a function to calculate the modulo of two numbers using the % operator and prints the result.
# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
f = lambda a, b: a + b
print("Sum is:", f(a, b))
```

## Output

<img width="453" height="248" alt="image" src="https://github.com/user-attachments/assets/1718e87e-603e-4c8b-aa4c-2c5718318865" />


## Result
The program successfully uses a lambda function to add two numbers and prints the result.
# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
def fact(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * fact(n - 1)


rows = int(input("Enter number of rows: "))


for n in range(rows):
    print(" " * (rows - n), end="")

    for k in range(n + 1):
       
        value = fact(n) // (fact(k) * fact(n - k))
        print(value, end=" ")

    print()

## Sample Output

<img width="524" height="398" alt="image" src="https://github.com/user-attachments/assets/4e6b7f50-50f8-4603-8fd0-d35bb88af2ef" />


## Result
The program successfully generates Pascal’s Triangle for the given number of rows using the combination formula.
## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input("Enter a number: "))
temp = num
rev = 0


while temp > 0:
    rev = (10 * rev) + (temp % 10)
    temp = temp // 10


if rev == num:
    print("The number is a Palindrome")
else:
    print("The number is not a Palindrome")
```
## Output

<img width="501" height="203" alt="image" src="https://github.com/user-attachments/assets/0e2716fe-9c34-4aac-bcf6-ae69cab0526f" />


## Result
The program successfully checks whether a given number is a palindrome by reversing it using a loop and comparing it with the original number.
