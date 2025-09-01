# Recursion:-

Recursion is when a function calls itself to solve a problem.

## Key Points:-
- The function solves smaller pieces of the problem each time.  
- It must have a **base case** to stop calling itself.

## Example: Factorial of 5
Factorial of 5 → 5 × 4 × 3 × 2 × 1

### Python Code

```python
def factorial(n):
    if n == 0:      # Base case
        return 1
    else:
        return n * factorial(n-1)  # Function calls itself

print(factorial(5))  # Output: 120
```

---

# Iteration:-

Iteration is when a block of code repeats multiple times using loops (`for` or `while`).

## Key Points:-
- No function calls itself.  
- Loop repeats until a condition becomes `False`.

## Example: Factorial of 5 using a Loop

### Python Code

```python
def factorial_iter(n):
    result = 1
    for i in range(1, n+1):
        result *= i
    return result

print(factorial_iter(5))  # Output: 120
```

---

# Difference Between Recursion and Iteration

| Feature       | Recursion                 | Iteration                     |
|---------------|---------------------------|-------------------------------|
| How it works  | Function calls itself     | Repeats code using loops      |
| Stop          | Base case                 | Condition becomes False       |
| Memory        | Uses stack (more memory)  | Constant memory               |
| Best for      | Problems with smaller sub-problems | Simple repeated tasks |

---

# Examples: Iteration vs Recursion

## Iteration: Factorial

```python
def factorial_iter(n):
    result = 1
    for i in range(1, n+1):
        result *= i
    return result

print(factorial_iter(5))  # Output: 120
```

## Recursion: Factorial
```python
def factorial_rec(n):
    if n == 0:
        return 1
    else:
        return n * factorial_rec(n-1)

print(factorial_rec(5))  # Output: 120
```

✅ Both give the same result, but iteration uses less memory.

---

# When to Use Recursion

- **Hierarchical Data** → Trees, Graphs  
- **Divide & Conquer Algorithms** → Merge Sort, Quick Sort  
- **Backtracking Problems** → Sudoku, N-Queens  
- **Problems Naturally Defined Recursively** → Factorial, Fibonacci, Tower of Hanoi

---

# When to Use Iteration

- **Simple Repetition** → Summing numbers, looping over arrays  
- **Performance Matters** → Avoid recursion overhead and stack overflow  
- **Memory Efficiency** → Iteration uses constant memory

---

# Quick Rule of Thumb

- **Use Recursion** → When the problem is naturally recursive (trees, divide & conquer, backtracking).  
- **Use Iteration** → When the problem is linear, involves simple repetition, or performance/memory is important.
