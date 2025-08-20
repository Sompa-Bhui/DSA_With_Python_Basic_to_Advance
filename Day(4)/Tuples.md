## 📘 Python Tuples
A tuple is an ordered, immutable collection in Python that can store items of the same or different data types, written with ().

### 1. What is a Tuple?
* A tuple is an ordered collection of items.
* Tuples are immutable → once created, you cannot change (add, remove, update) elements.
* Defined using parentheses ().

```python
t = (1, 2, 3)
print(t)        # (1, 2, 3)
```

### 2. Creating Tuples
```python
# Empty tuple
t1 = ()

# Single element tuple (must add comma)
t2 = (5,)     

# Multiple elements
t3 = (10, 20, 30)

# Mixed data types
t4 = (1, "hello", 3.14)

# Nested tuple
t5 = (1, (2, 3), (4, 5))
```

### 3. Indexing & Slicing
```python
nums = (10, 20, 30, 40, 50)

print(nums[0])    # 10
print(nums[-1])   # 50
print(nums[1:4])  # (20, 30, 40)
```

### Immutability
```python
nums = (1, 2, 3)
# nums[0] = 10   ❌ Error (cannot update)
# nums.append(4) ❌ Error (cannot add)

# ✅ But you can create a new tuple
nums = nums + (4, 5)
print(nums)  # (1, 2, 3, 4, 5)
```

### 5. Tuple Methods
```python
nums = (1, 2, 2, 3, 4)

print(nums.count(2))   # 2 (occurrences of 2)
print(nums.index(3))   # 3 (first index of 3)
```

### 6. Iterating Over Tuples
```python
fruits = ("apple", "banana", "mango")

for f in fruits:
    print(f)
```

### 7. Tuple Packing & Unpacking
```python
# Packing
person = ("Alice", 25, "Engineer")

# Unpacking
name, age, job = person
print(name)  # Alice
print(age)   # 25
print(job)   # Engineer
```

### 8. Nested Tuples
```python
matrix = ((1,2,3), (4,5,6), (7,8,9))

print(matrix[0])     # (1, 2, 3)
print(matrix[1][2])  # 6
```

### 9. Tuple vs List

| Feature    | List (`[]`)            | Tuple (`()`)                         |
|------------|------------------------|---------------------------------------|
| Mutability | Mutable                | Immutable                             |
| Performance| Slower                 | Faster (because fixed size)           |
| Methods    | Many (`append`, `remove`, etc.) | Few (`count`, `index`)        |
| Use cases  | Data that changes      | Fixed data, constants, dictionary keys |

### 10. Advanced Usage
* Tuples can be used as keys in dictionaries (lists cannot, because they are mutable).
* Useful when you want to store constant data.
```python
# Tuple as dictionary key
locations = {
    (28.61, 77.23): "Delhi",
    (19.07, 72.87): "Mumbai"
}

print(locations[(28.61, 77.23)])  # Delhi

Tuple = Address (latitude, longitude)

Dictionary = Map

So, when you give the address (28.61, 77.23), the map returns "Delhi" 🚏
```

---

## Summary:-
A built-in data type that lets us create im-mutable sequencs of values.

```python
tup = (87, 64, 33,95,76)   #tup[0], tup[1]..
tup[0]=43    #Not allowed in python
```
* tup1 = ()
* tup2 = (1,)
* tup3 = (1,2,3)

### Tuples Methods:-
tup = (2,1,3,1)

* tup.index(el)   #returns index of first occurrence  tup.index(1) is 1
* tup.count(el)   #counts total occurrences tup.count(1) is 2
