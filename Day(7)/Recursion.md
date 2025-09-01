# Recursion
Recursion is a programming technique where a function solves a problem by calling itself, usually with a smaller or simpler input, and has a base case to stop.

## What is Recursion?
Recursion is when a function calls itself to solve a problem.

## Key Points

- **Base Case:** Every recursive function must have a base case. This is where the function stops calling itself.  
- **Stack Overflow:** Without a base case, the function will run forever and cause a stack overflow.

## Basic Structure

```python
def function_name(parameters):
    if base_condition:      # Stop condition
        return result
    else:
        return function_name(modified_parameters)  # Recursive call
```

```python
def recursive_function(parameters):
    if base_condition:        # Base case
        return some_value
    else:
        # Recursive call
        return recursive_function(modified_parameters)
```

## Example 1: Factorial

Factorial of n:  

\[
n! = n \times (n-1) \times ... \times 1
\]

### Python Code

```python
def factorial(n):
    if n == 0:        # Base case
        return 1
    else:
        return n * factorial(n-1)  # Recursive call

print(factorial(5))  # Output: 120
```

## Example 2: Fibonacci Numbers

The Fibonacci sequence:  
0, 1, 1, 2, 3, 5, 8, ...

### Python Code

```python
def fibonacci(n):
    if n <= 1:  
        return n    # Base case
    else:
        return fibonacci(n-1) + fibonacci(n-2)  # Recursive call

for i in range(10):
    print(fibonacci(i), end=" ")
# Output: 0 1 1 2 3 5 8 13 21 34
```

## Example 3: Reverse a String

### Python Code

```python
def reverse_string(s):
    if s == "":
        return s    # Base case
    else:
        return reverse_string(s[1:]) + s[0]  # Recursive call

print(reverse_string("hello"))  # Output: "olleh"
```

## Advanced Recursion Concepts

### Tail Recursion
Tail recursion is when the recursive call is the last operation the function performs.  
It can help optimize memory usage in some languages that support tail call optimization.

### Python Code Example

```python
def tail_factorial(n, acc=1):
    if n == 0:
        return acc
    else:
        return tail_factorial(n-1, acc*n)

print(tail_factorial(5))  # Output: 120
```

## Advanced Recursion Concepts (Continued)

### Multiple Recursive Calls
Multiple recursive calls are useful in generating combinations, tree traversals, and similar problems.

#### Python Code Example

```python
def print_binary_strings(n, s=""):
    if n == 0:
        print(s)
    else:
        print_binary_strings(n-1, s + "0")
        print_binary_strings(n-1, s + "1")

print_binary_strings(3)
# Output:
# 000
# 001
# 010
# 011
# 100
# 101
# 110
# 111
```

## Summary:

### Recursion:-
When a function calls itself repeatedly.

#### Print n to 1 backwards
```python
def show(n):
    if(n == 0):   #Base case
        return
    print(n)
    show(n-1)
```

### Recursion in Factorial
```python
def fact(n):
    if(n == 0 or n == 1):
        return 1
    else:
        return n * fact(n-1)
```


