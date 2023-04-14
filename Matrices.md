# Matrices & List Comprehension
---
## What is a Matrix 
* We can create data structures with values in rows and columns (similar to a table)
  - this can be done by creating a list within a list 
* External libraries: There are external libraries and modules that can imported to help your program process 

---
## Matrix in python example 
```
matrix_A = [
  [1,2,3,4],
  [5,6,7,8]
  ]
# Accessing matrix A 
print(Row 1: %s' % matrix_A[0])
print('Value at Row 2 Column 2: %s' % matrix_A[1][1])

# output 
#Row 1: [1, 2, 3, 4]
#Value at Row 2 Column 2: 6
```

Rules of a regular matrix (a list within a list):
* All rows must have the same number of values
* All columns must have the same number of values
* All items in the 2D List must have the same data types
* Since indexing always starts at 0 ... row 1 is technically located at matrix_A[0]
---
## List comprehension
### What is it?: A concise method to create lists in python 

commonly used for:
*The list is a result of some operations applied to all its items
*It is a made from another sequence/iterable data
*The list is member of another list/sequence/iterable data that satisfies a certain condition

### Example 

```
# Previously used method 
squares = []
for i in range(10):
    squares.append(i ** 2)

print('Our result: %s' % squares)

# result: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

```
#New method 
squares = [i**2 for i in range(10)]

print('Our new result: %s' % squares)

# result: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```
