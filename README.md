# Some Python Hacks

### 1. List Comprehension


#### List based on some condition

```python
is_even = ["Yes" if not i%2 else "No" for i in range(10)]
print(is_even)
```
```
Output:
['Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No']
```
####  List of output of function

```python
def odd(even_no):
    return even_no+1
    
even_list = [i for i in range(20) if not i%2 ]    
odd_list=[odd(x) for x in even_list]
print(even_list)
print(odd_list)

```
```
Output:
[0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
[1, 3, 5, 7, 9, 11, 13, 15, 17, 19]
```

### 2. List Comprehension vs Generator Expression

Generator Expression is syntactically similar to List Comprehension, but are different based on memory uses. 
Generator Expression is memory efficient. It gives single object at a time while List Comprehension create a list of value.

When to use: For example is we need to add numbers 1 to aLargeNumber than if we use List Comprehension it create a list of size aLargeNumber but we don't need the list, we need only their sum, it is possible by Generator Expression

Syntax Difference: Use Parenthesis instead of square brackets.
```python
objec = (i for i in range(11) if i%2 == 0) 
print(objec) 

Output:
<generator object  at 0x000001452B1EEC50>
```


