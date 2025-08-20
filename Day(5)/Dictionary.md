## 📘 Python Dictionary
A dictionary in Python is an unordered, mutable collection of key-value pairs, written with {}.

### 1. What is a Dictionary?
* A dictionary is an unordered collection of items.
* It stores data in key : value pairs.
* Keys must be unique and immutable (e.g., string, number, tuple).
* Values can be of any type.

```python
student = {"name": "Sompa", "age": 21, "marks": 95}
print(student)
```

### 2. Creating Dictionaries
```python
# Empty dictionary
d = {}

# With data
person = {"name": "Bob", "age": 25}

# Using dict() function
data = dict(country="India", capital="Delhi")
```

### 3. Accessing Values
```python
student = {"name": "Sompa", "age": 21, "marks": 95}

print(student["name"])      # Sompa
print(student.get("age"))   # 21
print(student.get("city", "Not Found"))  # safe access with default
```

### 4. Adding & Updating
```python
student = {"name": "Sompa", "age": 21}

student["marks"] = 90        # add new key
student["age"] = 22          # update existing key

print(student)  # {'name': 'Sompa', 'age': 22, 'marks': 90}
```

### 5. Removing Items
```python
student = {"name": "Alice", "age": 22, "marks": 90}

student.pop("age")     # remove by key
student.popitem()      # remove last inserted item
del student["name"]    # delete using del
student.clear()        # remove all
```

### 6. Looping
```python
student = {"name": "Alice", "age": 22, "marks": 90}

# Loop through keys
for key in student:
    print(key)

# Loop through values
for value in student.values():
    print(value)

# Loop through key-value pairs
for key, value in student.items():
    print(key, ":", value)
```

### 7. Dictionary Methods
```python
student = {"name": "Alice", "age": 22}

print(student.keys())     # dict_keys(['name', 'age'])
print(student.values())   # dict_values(['Alice', 22])
print(student.items())    # dict_items([('name', 'Alice'), ('age', 22)])
```

### 8. Nested Dictionary
```python
students = {
    "101": {"name": "Alice", "marks": 95},
    "102": {"name": "Bob", "marks": 88}
}

print(students["101"]["name"])  # Alice
```

---


## Summary:- 
* Dictionary are used to store data values in key:value pairs
* They are unordered, mutuable(changeable) and don't allow to duplicate keys.

## "key" : value 

```python
dict = {
      "name" : Sompa",
      "cgpa" : 9,
      "marks" : [98,97,95],
}
```
* dict["name"], dict["cgpa"], dict["marks"]
* dict["key"] = "value"   #to asssign or add new

  ### Nested Dictionaries:-

  ```python
  student = {
        "name" : "Sompa",
        "score": {
            "math" : 100,
            "phy": 92,
            "chm" : 95
        }
    }
  ```

### Dictionary Methods:-

* myDict.keys()    #returns all keys
* myDict.values()  #returns all values
* myDict.items()   #returns all (key, val) pairs as tuples
* my.Dict("key")   #returns the key according to value
* my.Dict.update(newDict)  #insert the specified items to the dictionary.
