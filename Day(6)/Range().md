# 📘 Python `range()`

 -👉 range() in Python generates a sequence of numbers, used to control iteration in loops.

## 1. What is `range()`?

`range()` is a built-in Python function that generates a sequence of numbers.  

It is mostly used in `for` loops to iterate a fixed number of times.


## 2. Basic Syntax

```python
range(stop)               # 0 to stop-1
range(start, stop)        # start to stop-1
range(start, stop, step)  # start to stop-1 with step
```

## 3. Examples

### ✅ Example 1: Basic `range(stop)`

```python
for i in range(5):  # 0, 1, 2, 3, 4
    print(i)
```

### ✅ Example 2: range(start, stop)
```python
for i in range(2, 6):  # 2,3,4,5
    print(i)
```

### ✅ Example 3: range(start, stop, step)
```python
for i in range(1, 10, 2):  # 1,3,5,7,9
    print(i)
```

### 4. Negative Step
```python
for i in range(10, 0, -2):  # 10,8,6,4,2
    print(i)
```

### 5. Using range() with lists
```python
fruits = ["apple", "banana", "mango"]
for i in range(len(fruits)):
    print(i, fruits[i])
```

### 6. Converting range() to list, tuple, or set
```python
print(list(range(5)))   # [0,1,2,3,4]
print(tuple(range(3,7)))  # (3,4,5,6)
print(set(range(1,10,3))) # {1,4,7}
```

### 7. Advanced Tricks
```python
✅ 1. Sum of first n numbers
print(sum(range(1, 6)))  # 1+2+3+4+5 = 15
```

### ✅ 2. Reverse loop
```python
for i in range(5, 0, -1):
    print(i)  # 5,4,3,2,1
```

### ✅ 3. Nested loops with range()
```python
for i in range(1, 4):
    for j in range(1, 3):
        print(i, j)

# Output:
# 1 1
# 1 2
# 2 1
# 2 2
# 3 1
# 3 2
```

### 8. Key Points

* range() generates numbers on the fly (lazy evaluation), it doesn’t store all numbers in memory.

* Works perfectly with for loops, but not directly iterable in mathematical operations (need list() if required).

* Step can be positive or negative.

  ---

# Summary:-
Range functions returns a sequence of numbers, strating from 0 by default, and increments by 1(by default), and stops before a specified number.

- range(start?, stop, step?)

```python
for el in range(5):
    print(el)

for el in range(1, 5):
    print(el)
for el in range(1, 5, 2):
    print(el)
```



