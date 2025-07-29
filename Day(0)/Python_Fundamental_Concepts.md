# 🐍 Python: Fundamental Concepts

Pythons have 3 Fundamental Concepts
1) Comments
2) Identation
3) Statements

---

## 1️⃣ Comments

- Comments are used to explain code and **improve readability**.
- Make the source code readable and understandable by users.
- To explain the logic of code.
- Comments are generally ignored by Compilers and Interpreters.

### ➤ Single-Line Comment:
* Start with a Hash Symbol.
* The hash line must appear at the start of each line Comments.
```python
Eg:- This is a single-line comment
```
### ➤ Multi-Line Comment:
Can write comment of multiple lines using hash at the beginning of each line
```python
Eg:- #This is multi-line comments
       #Comment in Python
       #Using the single line
       # Commit Consecutively
```

### ➤ Doc String:
* Comments spans within multiple lines.
* Ignores everything in quotation marks.
* This is called Doc String.
* Written using 3 Single/Double quotes.
```python
Eg:- """ You can write Doc String like this"""
    ''' You can also write doc string like this'''
```


## 2️⃣ Indentation
- Python use identation to "highlight the **Block of Code**".
- Whitespace is used for identation in Python.
- All Statements with the "Same distance to the right" belong to the same block of code (4 Spaces).

### 🔹 Why is Indentation Important?

Unlike languages like C, C++, or Java which use `{}` to define blocks, Python uses **whitespace (indentation)** to group statements.

> 🧠 **Wrong indentation = Syntax Error (IndentationError)**


### ✅ Correct Example:
```python
if 5 > 2:
    print("5 is greater than 2")
    print("This is inside the if block")

print("This is outside the block")
  ```
### ❌ Incorrect Example (will raise IndentationError):
```python
if 5 > 2:
print("5 is greater than 2")   # ❌ Missing indentation
```

### 🔍 Summary of Identation:
Rules:
* Required	Indentation is mandatory in Python
* Default Standard	Use 4 spaces
* Don’t mix	Don’t mix tabs and spaces
* Shows logical grouping	Defines code blocks like if, for, def, etc.
* Error if wrong	Incorrect indentation → IndentationError

## 2️⃣ Statements
- Statements are Simple Codes written for execution.
- In Python, a **statement** is an instruction that the interpreter can execute.

> 🧠 Everything that **performs an action** — like assigning a value, calling a function, or looping — is a statement.


### 🔹 Types of Statements in Python:
There are three types of statements..

#### ✅ 1. **Simpe Statements**
A simple statement is **written in a single line** and performs a single action.

```python
x = 10
print("Hello, Python!")
```
🔹 These are the most common, like:
* Assignments (x = 5)
* Function calls (print())
* import statements (import math)

#### ✅ 2. Compound Statement
A compound statement contains multiple lines of code grouped by indentation and often includes control structures.
```python
if x > 0:
    print("Positive")
    x -= 1
```
🔹 Compound statements include:
* if, elif, else
* for, while loops
* try, except
* def, class
Each compound statement starts with a header line ending with a colon :, followed by an indented block (called a suite).

#### ✅ 3. Empty Statement (Pass)
When a statement is syntactically required but you don’t want any code to run, you use the pass statement.
```python 
def future_feature():
    pass  # Placeholder for future code
```
* In empty functions or classes.
* As a placeholder during development.
* To avoid syntax errors where a block is required.

  ### 🔍 Summary Table

| Statement Type   | Structure          | Example                    |
|------------------|--------------------|----------------------------|
| Simple           | One-line action    | `x = 10`                   |
| Compound         | Multi-line block   | `if`, `for`, `def`, `class` |
| Empty (`pass`)   | Does nothing       | `pass`                     |


 🧠 **Note:**  
* Python uses **indentation** to group compound statements  
* Python enforces readability by requiring proper indentation.
* If indentation is wrong, you'll get IndentationError.
* Python code is usually cleaner and more organized than languages that use {}.
