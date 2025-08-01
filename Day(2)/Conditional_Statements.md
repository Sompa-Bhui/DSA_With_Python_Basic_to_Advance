# ✅ What are Conditional Statements?

Conditional statements allow your program to make decisions based on conditions.

### 🧠 Real-life Examples:
- If it’s raining, take an umbrella.
- If you are hungry, eat food.

---

### 🐍 In Python, we use:

- `if`
- `elif` (short for **else if**)
- `else`

---

### 💻 Python Syntax Example:

```python
weather = "rainy"
hunger = True

if weather == "rainy":
    print("Take an umbrella.")
elif hunger:
    print("Eat food.")
else:
    print("Enjoy your day!")
```
## 🟢 Basic Syntax of `if`

```python
if condition:
    # code to run if condition is True
```
### 🧪 Example:

```python
age = 18

if age >= 18:
    print("You are an adult.")
```
## 🟡 `if...else` Statement

```python
if condition:
    # runs if condition is True
else:
    # runs if condition is False
```

### 🔍 Example:

```python
age = 16

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

## 🟠 `if...elif...else` Statement

Used when you have multiple conditions.

```python
if condition1:
    # runs if condition1 is True
elif condition2:
    # runs if condition2 is True
else:
    # runs if none of the above are True
```

### 🔍 Example:

```python
marks = 75

if marks >= 90:
    print("Grade: A")
elif marks >= 75:
    print("Grade: B")
elif marks >= 60:
    print("Grade: C")
else:
    print("Grade: F")
```

## 🧠 Nested `if` Statements

You can put one `if` inside another.

```python
age = 25
has_license = True

if age >= 18:
    if has_license:
        print("You can drive.")
    else:
        print("Get a license first.")
else:
    print("You are too young to drive.")
```
## 🎯 Ternary Operator (One-line `if...else`)

```python
result = "Pass" if marks >= 40 else "Fail"
print(result)
```
## 💡 NOTE:-

- ✅ **Indentation is critical** (use 4 spaces or a tab)
- ✅ **Keep conditions clear** and avoid too much nesting
- ✅ Use `elif` to avoid writing many `if...else` blocks
- ✅ Use `and`, `or`, `not` smartly to simplify logic


## ✅ Summary Table

| Type              | Example                                  |
|-------------------|------------------------------------------|
| Simple `if`       | `if x > 0:`                              |
| `if-else`         | `if x > 0: ... else:`                    |
| `if-elif-else`    | `if x > 90: ... elif x > 80: ... else:`  |
| Logical           | `if a > 0 and b < 5:`                    |
| Nested `if`       | `if a > 0: if b > 0:`                    |
| Ternary Operator  | `"Yes" if x > 0 else "No"`               |


