## 📘 Python Loops :
# 🔹 1. What is a Loop?

👉 A **loop** in Python is used to repeat a block of code multiple times until a condition is met.  

- Helps avoid writing the same code again and again.  
- Two main types of loops in Python:  
  1. **for loop**  
  2. **while loop**  

# 🔹 2. Types of Loops in Python

1. **for loop**  
   → Used when you know how many times you want to run the code.  

2. **while loop**  
   → Used when you want to repeat until a condition becomes false.  

# 🔹 3. for Loop

✅ **Syntax:**

```python
for variable in sequence:
    # code block
```

✅ **Example 1: Loop through a list**

```python
fruits = ["apple", "banana", "mango"]

for f in fruits:
    print(f)
# Output:
# apple
# banana
# mango
```

✅ **Example 2: Using `range()`**

```python
for i in range(5):   # 0 to 4
    print(i)
# Output: 0 1 2 3 4
```

✅ **Example 3: Custom `range()`**

```python
for i in range(2, 10, 2):  # start=2, stop=10, step=2
    print(i)
# Output: 2 4 6 8
```

# 🔹 4. while Loop

✅ **Syntax:**

```python
while condition:
    # code block
```

✅ **Example 1: Basic**

```python
count = 1
while count <= 5:
    print("Count:", count)
    count += 1
```

✅ **Example 2: Infinite loop (⚠ be careful)**

```python
while True:
    print("Running...")
    break   # stop loop using break
```

# 🔹 5. Loop Control Statements

✅ **`break` → exit loop immediately**

```python
for i in range(1, 6):
    if i == 3:
        break
    print(i)
# Output: 1 2
```

✅ **`continue` → skip current iteration**

```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
# Output: 1 2 4 5
```

✅ **`pass` → do nothing (placeholder)**

```python
for i in range(3):
    pass   # useful when writing empty loops
```

# 🔹 6. Nested Loops

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

# 🔹 7. Loop with else (special feature in Python)

```python
for i in range(5):
    print(i)
else:
    print("Loop finished without break")
```
# 🔹 3. Key Differences: `for` vs `while`

| Feature   | `for` loop                     | `while` loop                     |
|-----------|--------------------------------|----------------------------------|
| **Usage** | Iterates over a sequence       | Runs until condition becomes False |
| **Best for** | Known number of iterations  | Unknown number of iterations     |
| **Syntax** | `for var in sequence:`        | `while condition:`               |
| **Example** | `for i in range(5):`         | `while x < 5:`                   |

---

## Summary:-


## Loops in Python
Loops are used to repeat instructions.

### While Loops:-

while condition:
  #some work

## Break and Continue:-

### Break:-
Used to terminate the loop when encountered.

### Continue:
Terminates execution in the current iteration & continues executions of the loop with the next iteration.

## For Loop:-
* For loops are used for sequential traversal.
* For traversing list, string, tuples etc.

  for el in list
    #### #somework
```python
list = [1,2,3]
for el in list:
  print(el)
```

* for loop with else:
  for el in list:
  #### #someworks
  else:
    #### #works when loop ends
```python
for el in list:
    print(el)
else:
    print("End")
```



