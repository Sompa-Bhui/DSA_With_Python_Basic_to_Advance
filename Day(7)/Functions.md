# 📘 Python Functions 

## 🔹 1. What is a Function?

👉 **Definition:**  
A function in Python is a block of reusable code that performs a specific task.

✅ **Benefits of Using Functions:**
- Avoids repetition (**DRY – Don’t Repeat Yourself**)  
- Makes code **readable & modular**  
- Easier to **test and debug**  

## 🔹 2. Types of Functions

### ✅ Built-in Functions
These are already available in Python.  
Examples:  
```python
print("Hello, World!")
len([1, 2, 3, 4])
sum([5, 10, 15])
type(42)
```

## 🔹 3. Defining a Function

✅ **Syntax:**

```python
def function_name(parameters):
    """docstring (optional)"""
    # code block
    return value
```

## 🔹 3. Defining a Function

✅ **Syntax:**

```python
def function_name(parameters):
    """docstring (optional)"""
    # code block
    return value
```

## 🔹 4. Function Parameters

### 1️⃣ Positional Arguments
These are passed in the correct order to the function.

```python
def add(a, b):
    return a + b

print(add(5, 3))  # Output: 8
```

## 🔹 4. Function Parameters

### 1️⃣ Positional Arguments
These are passed in the correct order to the function.

```python
def add(a, b):
    return a + b

print(add(5, 3))  # Output: 8
```

## 🔹 4. Function Parameters

### 1️⃣ Positional Arguments
These are passed in the correct order to the function.

```python
def add(a, b):
    return a + b

print(add(5, 3))  # Output: 8
```

## 🔹 4. Function Parameters

### 1️⃣ Positional Arguments
These are passed in the correct order to the function.

```python
def add(a, b):
    return a + b

print(add(5, 3))  # Output: 8
```

## 🔹 4. Function Parameters

### 1️⃣ Positional Arguments
These are passed in the correct order to the function.

```python
def add(a, b):
    return a + b

print(add(5, 3))  # Output: 8
```

## 🔹 5. Return vs Print

```python
def square(x):
    return x * x

print(square(5))   # Output: 25
```

## 🔹 6. Scope of Variables

- **Local Variable** → Defined **inside** a function, can’t be accessed outside.  
- **Global Variable** → Defined **outside** a function, accessible everywhere.  

```python
x = 10  # global variable

def show():
    y = 5  # local variable
    print(x, y)  # Accessible inside the function

show()

# print(y)  # ❌ ERROR: 'y' is not defined outside the function
```

## 🔹 7. Lambda Functions (Anonymous Functions)

👉 Short, one-line functions created using the **`lambda`** keyword.

```python
square = lambda x: x * x
print(square(6))  # Output: 36
```

## 🔹 8. Advanced – Higher Order Functions

👉 Functions that either **take another function as input** or **return a function**.

```python
def apply(func, x):
    return func(x)

print(apply(lambda n: n**3, 4))  # Output: 64
```

## 🔹 9. Recursion

👉 A function that **calls itself** to solve a problem.

```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)

print(factorial(5))  # Output: 120
```

## 🔹 10. Decorators (Advanced)

👉 Special functions that **modify or extend the behavior** of other functions without changing their code.

```python
def decorator(func):
    def wrapper():
        print("Before function")
        func()
        print("After function")
    return wrapper

@decorator
def hello():
    print("Hello!")

hello()
```

## Summary

## ✅ Quick Summary

- **Function** = A block of reusable code.  
- Supports → **parameters, return values, recursion, lambda, decorators**.  
- Helps in writing **clean, reusable, and modular code**.  

