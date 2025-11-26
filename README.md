# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using *list comprehension*, and stores them in a list.

---

## 🧠 ALGORITHM:

1. *Start*
2. Create a class named program
3. Create variables a, b, and c to represent:
   - a: Lower limit
   - b: Step value
   - c: Upper limit
4. Initialize the values using a constructor __init__
5. Define a method display() that uses *list comprehension* to store even numbers
6. Print the resulting list of even numbers
7. *Stop*

---

## 💻 PROGRAM:
```
class generate:
    def __init__(self,first,d,last):
        self.first=first
        self.d=d
        self.last=last
    def Ap_generate(self):
        l=[i for i in range(self.first,self.last+1,self.d)]
        return l
series=generate(200,2,301)
print(series.Ap_generate())
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/236e72c7-e79e-4458-b4bf-8be1fb0dd279)

## RESULT:
         Thus, the Python class-based program that generates all even numbers between 200 and 300 using *list comprehension*, and stores them in a list.

# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
Write a Python class program to store all odd numbers between 500 and 600 in a reverse order  using list comprehension

---

## 🧠 ALGORITHM:

1. *Start*
2. Create variables r and c to represent the number of rows and columns of the matrix.
3. Get the values of r and c from the user.
4. Define a function create(r, c) to create the matrix by reading the elements from the user.
5. Use *list comprehension* to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. *Stop*

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
      Thus ,the Python program to compute the *transpose* of a matrix using *list comprehension*.

# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints *only the diagonal elements*, leaving other elements blank in the output.

## 📌 Aim

To write a Python program to read matrix [3x3] that print the major(main) and minor(off) diagonal elements.
## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size rows × columns.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If i == j, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥 Program
```
l=[list(map(int,input().split())) for _ in range(3)]
print("Matrix:")
for i in l:
    print(*i)
mad=[]
mid=[]
k=len(l[0])-1
for i in range(len(l)):
    for j in range(len(l[i])):
        if i==j:
            mad.append(l[i][j])
        if j==k:
            mid.append(l[i][j])
    k-=1
print("Major Diagonal Elements : ",(*mad))
print("Minor Diagonal Elements : ",(*mid))
```
### Output:
![image](https://github.com/user-attachments/assets/78235dd3-d15c-4430-989d-4bb7bc582861)


## Result
     Thus the Python program to read matrix [3x3] that print the major(main) and minor(off) diagonal elements.

# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python Program to subtract two matrices by reading the matrix from the user.

---

## 🧠 ALGORITHM:

1. *Start*
2. Create variables r and c for rows and columns
3. Get the values of r and c from the user
4. Define a function create_matrix(n, m) to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the create_matrix() function twice to read two matrices A and B
6. Define a loop to subtract the elements of matrix B from matrix A
7. Store the result in a new matrix C
8. Print the resulting matrix C
9. *Stop*

---

## 💻 PROGRAM:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M
r,c=input().split()
A=create_matrix(int(r),int(c))
B=create_matrix(int(r),int(c))
C=[]
for i in range(int(r)):
    R=[]
    for j in range(int(c)):
        item=A[i][j]-B[i][j]
        R.append(item)
    C.append(R)
print(A)
print(B)
print(C)
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c13e49c9-e679-4b64-85af-4df96445863d)

## RESULT:
      Thus ,the Python Program to subtract two matrices by reading the matrix from the user.

# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the *Insertion Sort algorithm* using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the *Insertion Sort* algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. *Start the program*
2. *Define a class* InsertionSorter
3. Inside the class:
   - create_list():
     - Read number of elements
     - Store them in a list
   - insertion_sort():
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - print_list():
     - Print the sorted list
4. *Create an object* of the class
5. *Call* the methods in order: create_list(), insertion_sort(), and print_list()
6. *End the program*

---

## 💻 PROGRAM:
```
class InsertionSorter:
    def __init__(self):
        self.lst = []

    def create_list(self):
        n = int(input("Enter the number of elements: "))
        print("Enter the elements:")
        for _ in range(n):
            val = int(input())
            self.lst.append(val)

    def insertion_sort(self):
        for i in range(1, len(self.lst)):
            key = self.lst[i]
            j = i - 1
            while j >= 0 and key < self.lst[j]:
                self.lst[j + 1] = self.lst[j]
                j -= 1
            self.lst[j + 1] = key

    def print_list(self):
        print("Sorted list:", self.lst)

sorter = InsertionSorter()
sorter.create_list()
sorter.insertion_sort()
sorter.print_list()
```

## OUTPUT:
```
Enter the number of elements: 5
Enter the elements:
23
12
45
8
19
Sorted list: [8, 12, 19, 23, 45]
```
## RESULT:
Hence Insertion Sort using a Python class is done.
