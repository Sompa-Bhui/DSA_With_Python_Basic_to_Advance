# 🆔 Python Identifiers

An identifier is a name used to identify a **variable**, **function**, **class**, or other **objects** in Python.

🟢 **Note:** *Variable* is only one kind of identifier.  
Other kinds include **function names**, **class names**, **structure names**, etc.



📌 All **variables** are **identifiers**, but the **vice-versa is not always true**.


## ✅ Valid Identifier Examples
```
name = "Moni"               #'name' is an identifier (variable)

total_marks = 95            #valid identifier with underscore

def greet():                #'greet' is an identifier (function)
  
class Student:              #'Student' is an identifier (class)
```




## 🧠 Python Identifier Rules (Important)

| Rule | Explanation | Example |
|------|-------------|---------|
| ✅ Must begin with a letter (A-Z or a-z) or an underscore `_` | Identifier must start with an alphabet or underscore | `my_var`, `_hidden` |
| ✅ Can contain letters, digits (0-9), and underscores `_` | Alphanumeric characters and `_` are allowed | `data123`, `student_marks` |
| ❌ Cannot begin with a digit | Identifiers cannot start with a number | `2name` ❌ |
| ❌ Cannot use special symbols like `@`, `#`, `-`, `!` | Special characters are not allowed | `my-name`, `total@value` ❌ |
| ❌ Cannot be a reserved keyword in Python | Keywords like `if`, `class`, `for`, etc. are not allowed | `if = 10`, `class = "abc"` ❌ |



### 🔑 Important Notes:

- **Keywords** are already defined by Python. You **can’t use them as identifiers**.

> ❌ Example of Python Keywords (cannot be used as variable/function/class names):  
`False`, `None`, `True`, `and`, `or`, `if`, `else`, `class`, `def`, `return`, `while`, `for`

### 🔠 Python Identifiers are Case-Sensitive:

```python
Age = 21
age = 18
```
Age and age both are not same

