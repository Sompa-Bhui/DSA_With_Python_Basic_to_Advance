# 🔹 While Loop

👉 **Definition:**  
A `while` loop executes a block of code as long as a condition is `True`.

### ✅ Syntax:
```python
while condition:
    # code block
```

✅ **Example 1: Counting**

```python
count = 1
while count <= 5:
    print("Count:", count)
    count += 1
# Output: Count: 1 … Count: 5
```

✅ **Example 2: Infinite Loop (⚠ careful)**

```python
while True:
    print("Running...")
    break   # break to avoid infinite loop
```

✅ **Example 3: While with user input**

```python
password = ""
while password != "python123":
    password = input("Enter password: ")
print("Access Granted ✅")
```

👉 **Use case:**

- When you don’t know how many times the loop should run.  
- Runs until a condition becomes `False`.  
