## 🧠 What is a Function?

A **function** in Python is a block of reusable code that performs a specific task.

- 🔁 It runs **only when called**.
- 📦 It helps **avoid repetition**.
- 🧩 It makes code **modular and organized**.

## 📌 1. Defining a Function

### ✅ Syntax:

```python
def function_name():
    # code block
```
### 🧪 Example:
```python
def say_hello():
    print("Hello! Welcome to Python.")

say_hello()  # Call the function
```

## 📌 2. Function with Parameters (Inputs)

You can pass values to a function using parameters.

### ✅ Syntax:

```python
def greet(name):
    print("Hello", name)
```
### 🧪 Example:
```python
greet("Sompa")      # Output: Hello Sompa
greet("Biplab")   # Output: Hello Biplab
```

## 📌 3. Function that Returns a Value

Use the `return` keyword to send back a result.

### ✅ Example:

```python
def square(x):
    return x * x

result = square(5)
print("Square is:", result)  # Output: 25
```

## 📌 4. Multiple Parameters

Functions can take more than one input:

```python
def add(a, b):
    return a + b

print(add(10, 20))  # Output: 30
```

## 📌 5. Default Parameters

You can assign default values to parameters — useful when you don’t always want to pass a value.

```python
def greet(name="Guest"):
    print("Hello", name)

greet()           # Output: Hello Guest
greet("Aisha")    # Output: Hello Aisha
```

## 📌 6. Keyword Arguments

You can call functions using parameter names, so the order doesn’t matter.

```python
def student_info(name, age):
    print(f"Name: {name}, Age: {age}")

student_info(age=18, name="Usman")
```

## 📌 7. Returning Multiple Values

Python allows returning more than one value from a function:

```python
def get_stats(x, y):
    return x + y, x - y, x * y

sum_, diff, prod = get_stats(10, 5)
print("Sum:", sum_, "Difference:", diff, "Product:", prod)
```

## 📌 8. Functions and Loops

You can call functions inside a loop:

```python
def is_even(n):
    return n % 2 == 0

for i in range(1, 6):
    if is_even(i):
        print(i, "is even")
```

## 📌 9. List + Function Example

```python
def print_items(items):
    for item in items:
        print(item)

fruits = ["apple", "banana", "cherry"]
print_items(fruits)
```

## 📌 10. Variable-Length Arguments

Sometimes you don't know how many inputs you'll get.

### 🔹 `*args` (for multiple positional arguments)

```python
def total(*numbers):
    sum = 0
    for num in numbers:
        sum += num
    return sum

print(total(1, 2, 3, 4))  # Output: 10
```
* *args gives you a tuple of all values.

### 🔹 **kwargs (for multiple named arguments)
```python
def profile(**info):
    for key, value in info.items():
        print(key, ":", value)
profile(name="Ali", age=22, city="Lahore")
```
* **kwargs gives you a dictionary of all named arguments.

## 📌 11. Lambda Functions (Anonymous/One-line Functions)
Lambda functions are short functions without a name.

``` python
square = lambda x: x * x
print(square(5))  # Output: 25
```

### Another example:

```python
add = lambda a, b: a + b
print(add(2, 3))  # Output: 5
```
* Useful in data processing, sorting, filtering, etc.

## ✅ Summary Table

| Feature                  | Example                  |
|--------------------------|--------------------------|
| Define a function        | `def hello():`           |
| Call a function          | `hello()`                |
| Function with input      | `def greet(name):`       |
| Function with output     | `return x + y`           |
| Default parameter        | `def greet(name="Guest")`|
| Return multiple values   | `return a, b, c`         |
| Variable arguments       | `*args`, `**kwargs`      |
| One-line function        | `lambda x: x * 2`        |


## Parameter & Arguments:-

### ✅ Parameter 
A **parameter** is a variable in the function definition.

It acts as a **placeholder** for the value that will be passed in when the function is called.

📌 *Think of it as a label for the input expected by the function.*
```python
def greet(name):  # 'name' is a parameter
    print(f"Hello, {name}!")
```
## ✅ Parameter

A **parameter** is a variable in the function definition.

It acts as a **placeholder** for the value that will be passed in when the function is called.

📌 *Think of it as a label for the input expected by the function.*
```python
greet("Sompa")  # 'Sompa' is the argument
```
```python
def greet(name):  # "name" is a **parameter**
    print("Hello", name)
```
greet("Sompa")      # "Sompa" is an **argument**

## 📊 Summary Table

| Term      | Where it Appears           | What it Represents              |
|-----------|----------------------------|---------------------------------|
| Parameter | In the function definition | A placeholder name for input    |
| Argument  | In the function call       | The actual value passed in      |


