# Map and Filter in Python 
---
## Map function
* Map function is used to apply a function to iterable data 
* Does not return a specific datat type, instead an iterable datatype 
* use of the Map function should be followed by the list function 

### Example:
``` python 
def square(num):
    ''' squares the given num argument '''
    return num ** 2
# end of square

array = list(range(1,11))
square_array = list(map(square, array))

print('Original Array:', array)
print('Array Squared:', square_array)

# what it does is square all numbers in an iterbale data type 
#Original Array: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
#Array Squared: [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]

```
---

## Filter function 
* Used to filter out certain items from a data set 
* If an item meets a certain condition it can be removed

### Example of filter function 
```
def isOdd(x):
    ''' isOdd() returns True if x is odd.'''
    return x % 2 != 0

array = list(range(1,101))
odds = list(filter(isOdd, array))

print('Odd Numbers from 1 to 100:', odds)

# if a number in the data set is even (diviisable by 2) then it is filtered out of the data set
```

### Composition Functions:
* Using a function within a function
* Applying one function to the result of another function 
