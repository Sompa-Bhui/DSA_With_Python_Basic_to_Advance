## 📘 Python Sets
👉 A set in Python is an unordered collection of unique, mutable elements, written with {}.

## 1. What is a Set?
* A set is an unordered collection of unique items.
* Sets are mutable (you can add/remove items), but the items inside must be immutable (like numbers, strings, tuples).
* Sets do not allow duplicate values.

```python
my_set = {1, 2, 3, 3, 4}
print(my_set)  # {1, 2, 3, 4} (duplicate 3 removed)
```

## 2. Creating Sets
```python
# Empty set
s = set()   # {} is dictionary, not set!

# With values
nums = {10, 20, 30}

# Mixed data types
mix = {1, "apple", 3.14}

# From list/tuple
s2 = set([1, 2, 2, 3])
print(s2)   # {1, 2, 3}
```

### 3. Adding & Removing Items
```python
s = {1, 2, 3}

s.add(4)         # add single element
s.update([5, 6]) # add multiple elements

s.remove(2)      # remove (error if not exists)
s.discard(10)    # remove safely (no error)
s.pop()          # removes random element
s.clear()        # empty the set
```

### 4. Set Operations (Math-like)
```python
a = {1, 2, 3, 4}
b = {3, 4, 5, 6}

print(a | b)   # Union → {1, 2, 3, 4, 5, 6}
print(a & b)   # Intersection → {3, 4}
print(a - b)   # Difference → {1, 2}
print(a ^ b)   # Symmetric Difference → {1, 2, 5, 6}
```

### 5. Membership Test 
```python
s = {1, 2, 3}
print(2 in s)    # True
print(5 not in s) # True
```

### 6. Iterating
```python
fruits = {"apple", "banana", "mango"}
for f in fruits:
    print(f)
```

### 7. Useful Functions
```python
nums = {5, 1, 7, 2}

print(len(nums))     # size
print(max(nums))     # largest
print(min(nums))     # smallest
print(sum(nums))     # total sum
```

### 8. Frozen Set (Immutable Set)
```python
fs = frozenset([1, 2, 3, 2])
print(fs)       # frozenset({1, 2, 3})

# fs.add(4)  ❌ Error (cannot change frozenset)
```

### 9. Set Comprehension 
```python
squares = {x**2 for x in range(6)}
print(squares)  # {0, 1, 4, 9, 16, 25}
```

--- 

## Summary:-










# 🔥 Difference Between List, Tuple, Dictionary, and Set

| Feature     | List      | Tuple     | Dictionary           | Set           |
|-------------|-----------|-----------|----------------------|---------------|
| **Order**   | ✅ Ordered | ✅ Ordered | ❌ Unordered (keys)  | ❌ Unordered  |
| **Mutable** | ✅ Yes     | ❌ No      | ✅ Yes               | ✅ Yes        |
| **Duplicates** | ✅ Allowed | ✅ Allowed | Keys ❌, Values ✅  | ❌ Not Allowed |
| **Access by** | Index   | Index     | Key                  | No indexing   |




