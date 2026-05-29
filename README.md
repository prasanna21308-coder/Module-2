## Developed by: PRASANNA V (212225220072)

# 1.Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program

```
a = 16
b = bin(a)
 
print(a,"'s binary value is:",b)
```
## Output
<img width="335" height="38" alt="image" src="https://github.com/user-attachments/assets/a9d48a40-4260-4926-9532-3f2d1ba09187" />

## Result
Thus the program has been executed successfully.

# 2.Functions in Python: Modulo Calculator

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
def result(a,b):
    return a%b
    
x = 10
y = 3
print(x,"%",y,"=",result(x,y))
print()

a,b = map(int,input("Enter two numbers to perform Modulo operation: ").split())
print("Result of modulo operation:",result(a,b))
```
## Output
<img width="580" height="132" alt="image" src="https://github.com/user-attachments/assets/fdd1a53f-f2cc-404e-bc81-3ff894aeb937" />

## Result
Thus the program has been executed successfully.

# 3.Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
f = lambda x,y: x+y

a,b = map(int,input('Enter two numbers to return their sum: ').split())
print("Result of addition:",f(a,b))
```

## Output
<img width="486" height="67" alt="image" src="https://github.com/user-attachments/assets/eec3257c-3216-49b3-942e-2c081fa3e86a" />

## Result
Thus the program has been executed successfully.

# 4.🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

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
```
n = int(input("Enter number of rows to be printed: "))

for i in range(n):
    val = 1
    print(" " * (n - i - 1), end="")
    for j in range(i + 1):
        print(val, end=" ")
        val = val * (i - j) // (j + 1)
    
    print("")
```
## Sample Output
<img width="419" height="180" alt="image" src="https://github.com/user-attachments/assets/be3d4ef8-7988-434c-b88c-fca12b168076" />

## Result
Thus the program has been executed successfully.

## 5.Loops in Python: Palindrome Number Checker

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
num = int(input("Enter number to check if it is palindrome: "))

temp = num
rev = 0
while temp>0:
    rem = temp%10
    rev = rev*10+rem
    temp = temp//10

if rev==num:
    print(f"{num} is a palindrome")
else:
    print(f"{num} is not a palindrome")
```
## Output
<img width="507" height="74" alt="image" src="https://github.com/user-attachments/assets/4e484915-64b1-44f8-ac7f-ffdf51227f25" /><br>
<img width="494" height="70" alt="image" src="https://github.com/user-attachments/assets/1d21a71c-2c6c-43de-9532-8ac292dd8e61" />

## Result
Thus the program has been executed successfully
