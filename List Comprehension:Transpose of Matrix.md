# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
Write a Python class program to store all odd numbers between 500 and 600 in a reverse order  using list comprehension

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
```
class OddNumbers:
    def __init__(self):
        self.odd_numbers = [num for num in range(599, 499, -2)]
    
    def get_numbers(self):
        return self.odd_numbers

odd_numbers_instance = OddNumbers()

print(odd_numbers_instance.get_numbers())
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/bac77514-fc1a-4f71-851d-187999b39a41)

## RESULT:
      Thus ,the Python program to compute the **transpose** of a matrix using **list comprehension**.


