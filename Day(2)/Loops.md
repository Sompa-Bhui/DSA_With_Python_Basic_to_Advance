## 🔁 What are Loops?

Loops allow us to repeat a block of code multiple times.

### 🧠 For example:
- Printing numbers from 1 to 10  
- Processing each item in a list  
- Repeating a task until a condition is met  

---

### 🔄 Python has two main types of loops:

- `for` loop  
- `while` loop
  
## 🔷 1. `for` Loop (Definite loop)

Used when you know how many times to run the loop.

### 🧪 Syntax:
```python
for variable in sequence:
    # do something
```

## ✅ Example: Print numbers from 1 to 5
```python
for i in range(1, 6):
    print(i)
```
* range(1, 6) gives numbers: 1 2 3 4 5
* i is the loop variable

## 📌 range() Function
Used to generate a sequence of numbers.

```python
range(start, stop, step)
```
* range(5) → 0 to 4
* range(1, 6) → 1 to 5
* range(10, 0, -2) → 10, 8, 6, 4, 2

## ✅ Example: Print even numbers from 2 to 10
```python
for i in range(2, 11, 2):
    print(i)
```

✅ Looping through a list:
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

---

## 🔶 2. `while` Loop (Indefinite loop)

Used when you don't know how many times to repeat — runs as long as a condition is `True`.

### 🧪 Syntax:

```python
while condition:
    # do something
```
✅ Example: Print numbers from 1 to 5
```python
i = 1
while i <= 5:
    print(i)
    i += 1  # increment i by 1
```
* If you don’t update i, it will run forever (infinite loop).

### 🔄Some Importants Terms in Loop
## ⚙️ Loop Control Statements
🔸 break – stop the loop immediately
```python
for i in range(1, 10):
    if i == 5:
        break
    print(i)
# Output: 1 2 3 4
```

## 🔸 continue – skip current iteration, go to next
```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
# Output: 1 2 4 5
```

## 🔸 else with loop – runs only if loop ends normally
```python
for i in range(1, 5):
    print(i)
else:
    print("Loop finished!")
```
* If loop ends with break, else doesn't run.
---
## 🚨 Common Mistakes

| Mistake                      | What to Watch                          |
|-----------------------------|----------------------------------------|
| Infinite `while` loop       | Always update the condition variable   |
| Wrong range (e.g. `range(1, 10)`) | Doesn't include 10 (stop is exclusive) |
| Using `=` instead of `==` in condition | Use `==` for comparison              |

---

## 🔚 Summary

| Loop Type | Use When                   | Example                          |
|-----------|----------------------------|----------------------------------|
| `for`     | Fixed number of repeats    | `for i in range(5)`              |
| `while`   | Repeat until condition     | `while i < 5:`                   |
| `break`   | Exit loop early            | `if x == 5: break`               |
| `continue`| Skip current iteration     | `if x % 2 == 0: continue`        |
| `else`    | Run after loop completes   | `for i in ... else:`             |
