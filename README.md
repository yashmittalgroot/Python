# Sone Python Hacks

### 1. List based on some condition

```python
even_list = ["Yes" if not i%2 else "No" for i in range(10)]
print(even_list)
```
```
Output:
['Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No']
```

### 2. List of output of function on each element of array

Imagine you have an list and a function and you want output of function on each element of list than "map" is useful. 

```python
def odd(even_no):
    return even_no+1
    
even_list = [i for i in range(20) if not i%2 ]    
odd_list=list(map(odd,even_list))
print(odd_list)
```
