# 🧠 Input and Output in Python

**Input** = Taking information/data from the user  
**Output** = Showing information to the user on screen

---

## 📥 Input in Python

In Python, we use the `input()` function to get input from the user.

### 👉 Basic Example:

```python
name = input("Enter your name: ")
print("Hello,", name)
```
* input("Enter your name: ") shows the message to the user.
* Whatever the user types is saved in the name variable.
* print() then shows the output on the screen.

  ⚠️ Important:
* input() always gives a string (text), even if the user types a number.

  If you want a number, you have to convert it:

```python
age = int(input("Enter your age: "))
print("You are", age, "years old.")
```
* Here, int() converts the input string to an integer (number).

* You can also use float() if you need decimal numbers.
```python
price = float(input("Enter the price: "))
print("Price is", price)
```

---

## 📤 Output in Python

To display something, we use the `print()` function.

### 👉 Basic Example:

```python
print("Welcome to Python!")
```
You can print multiple things using commas:

```python
name = "Sompa"
age = 21
print("Name:", name, "Age:", age)
```


✅ **Using f-strings (Recommended)**  
This is a modern and cleaner way to format output:

```python
name = "Ali"
age = 25
print(f"My name is {name} and I am {age} years old.")
```
🔁 **Full Example:**

```python
name = input("What is your name? ")
age = int(input("How old are you? "))
print(f"Hello {name}, you are {age} years old!")
```
## 📝 Summary

| Task             | Code Example                                 |
|------------------|----------------------------------------------|
| Take input       | `name = input("Enter name: ")`               |
| Convert to int   | `age = int(input("Enter age: "))`            |
| Print output     | `print("Hello!")`                            |
| f-string output  | `print(f"Hi {name}")`                        |

