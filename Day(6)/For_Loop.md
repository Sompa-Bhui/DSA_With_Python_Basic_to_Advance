# 🔹 For Loop

👉 **Definition:**  
A `for` loop is used to iterate over a sequence (like **list, tuple, string, range, or set**) and execute code for each element.

### ✅ Syntax:
```python
for variable in sequence:
    # code block
```

✅ **Example 1: Iterating over a list**

```python
fruits = ["apple", "banana", "mango"]
for fruit in fruits:
    print(fruit)
# Output:
# apple
# banana
# mango
```

✅ **Example 2: Iterating over a string**

```python
for ch in "PYTHON":
    print(ch)
# Output: P Y T H O N
```

✅ **Example 3: Using `range()`**

```python
# range(start, stop, step)
for i in range(1, 6):  
    print(i)
# Output: 1 2 3 4 5
```

✅ **Example 4: Nested for loop**

```python
for i in range(3):
    for j in range(2):
        print(i, j)

# Output:
# 0 0
# 0 1
# 1 0
# 1 1
# 2 0
# 2 1
```

👉 **Use case:**

- When you know how many times to run the loop.  
- Used for iteration over sequences (**list, tuple, dictionary, string**).  




