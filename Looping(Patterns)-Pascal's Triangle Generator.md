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
```

import math

num_rows = int(input("Enter the number of rows for Pascal's Triangle: "))

for row in range(num_rows):
    print(" " * (num_rows - row - 1), end="")
    
    for col in range(row + 1):
        value = math.factorial(row) // (math.factorial(col) * math.factorial(row - col))
        print(value, end=" ")
    
    print()


```

## Sample Output
![image](https://github.com/user-attachments/assets/1d116a23-14ff-4248-9163-ba873247f355)

## Result
The code has been executed susscessfully.
