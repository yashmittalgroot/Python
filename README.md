# Sone Python Hacks

### 1. List based on some condition

```python
is_even = ["Yes" if not i%2 else "No" for i in range(10)]
print(even_list)
print(is_even)
```
```
Output:
['Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No']
```

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


