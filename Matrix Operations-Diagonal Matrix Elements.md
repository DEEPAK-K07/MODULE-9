# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program to read matrix [3x3] that print the major(main) and minor(off) diagonal elements.
## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
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
