# 📘 Python Module

## 🔹 What is a Module in Python?
A **module** in Python is simply a file with the extension `.py` that contains **Python code** such as:

- Functions  
- Variables  
- Classes  

## 🔹 Why Use Modules?
Modules help us:
- Avoid writing the same code again and again  
- Organize code into smaller, reusable parts  
- Make our programs easier to maintain and understand  

## 🔹 Types of Modules in Python

1. **Built-in Modules**  
   - These come with Python by default.  
   - Example:  
     ```python
     import math
     print(math.sqrt(16))   # Output: 4.0
     ```

2. **User-defined Modules**  
   - These are modules created by the programmer.  
   - Example:  
     ```python
     # mymodule.py
     def greet(name):
         return f"Hello, {name}!"
     ```

3. **Third-party Modules**  
   - These are modules developed by others and installed using `pip`.  
   - Example:  
     ```python
     # Install with: pip install requests
     import requests
     response = requests.get("https://api.github.com")
     print(response.status_code)
     ```

## 🔹 Third-party Modules Example:

These need to be installed using pip:

- **flask** → lightweight web framework  
- **django** → full-featured web framework  
- **numpy** → numerical computing  
- **pandas** → data analysis  
- **requests** → HTTP requests  


---

## 🔹 Example Usage
```python
# main.py
import mymodule
import math

print(mymodule.greet("Alice"))   # Output: Hello, Alice!
print(math.factorial(5))         # Output: 120
```

# 📦 pip (Python Package Installer)

## 🔹 What is pip?
`pip` stands for **Python Package Installer**.  
It is a tool used to **install, upgrade, and manage extra Python libraries** from the internet (usually from [PyPI](https://pypi.org/)).

---

## 🔹 Why Use pip?
- To extend Python's functionality by adding third-party libraries  
- To easily install and manage dependencies for projects  

---

## 🔹 Example: Installing a Package
```bash
pip install requests
```

# 🔍 Difference

- **Module** → one Python file (like `math`, `random`)  
- **Package** → collection of many modules (like `numpy`, `pandas`)  
- **pip** → the tool to download and install packages  
