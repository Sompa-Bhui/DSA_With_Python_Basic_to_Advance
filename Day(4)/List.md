# 📘 Python Lists

## 1. What is a List?
A **list** in Python is an **ordered, mutable collection** that can store multiple items of different data types.  

```python
marks = [87, 64, 33, 95, 76]   # marks[0], marks[1]...
student = ["Karan", 85, "Delhi"]  # student[0], student[1]...

student[0] = "Arjun"    # allowed in Python

print(len(student))   # returns length

```
## 2. Creating List

```python
# Empty list
a = []

# List of integers
nums = [1, 2, 3, 4, 5]

# Mixed data types
mixed = [1, "apple", 3.5, True]

# Nested list
nested = [1, [2, 3], [4, 5]]
```
## 3. Indexing & Slicing

```python
fruits = ["apple", "banana", "mango", "orange"]

# Indexing (starts from 0)
print(fruits[0])   # apple
print(fruits[-1])  # orange (last element)

# Slicing
print(fruits[1:3])   # ['banana', 'mango']
print(fruits[:2])    # ['apple', 'banana']
print(fruits[2:])    # ['mango', 'orange']
```
## 4. Common Methods
```python
fruits = ["apple", "banana", "mango"]

# Add element
fruits.append("orange")   # add at the end
fruits.insert(1, "grapes") # add at specific index

# Remove element
fruits.remove("banana")  # remove by value
fruits.pop()             # remove last element
fruits.pop(1)            # remove by index
del fruits[0]            # delete using del

# Update element
fruits[0] = "kiwi"

# Clear list
fruits.clear()
```

## 5. Useful Functions
```python
nums = [5, 2, 9, 1, 7]

print(len(nums))   # length
print(max(nums))   # largest value
print(min(nums))   # smallest value
print(sum(nums))   # sum of all elements

nums.sort()        # sort ascending
nums.sort(reverse=True)  # sort descending
nums.reverse()     # reverse order
```
## 6. Iterating Over Lists
```python
fruits = ["apple", "banana", "mango"]

# For loop
for f in fruits:
    print(f)

# With index
for i in range(len(fruits)):
    print(i, fruits[i])
```

## 7. Membership Test
```python
fruits = ["apple", "banana", "mango"]

print("apple" in fruits)     # True
print("cherry" not in fruits) # True
```

---
## Summary:-

### Differents Between List and String:-
* List :-Mutuable(Changeable)
* String :-Im-Mutuable(Unchangeable)

### List Slicing 
```python
list_name[starting_idx : ending_idx] #ending idx is not included
marks = [87, 64, 33, 95, 76]
marks[1:4] is [64, 33, 95]
marks[1: ] is same as marks[1: len(marks)]
marks[-3 : -1] is [33, 95]
```

## List Methods:-
```python
list = [2, 1, 3]
list.append(4)  #adds one element at the end [2,1,3,4] --> This is called mutating the list.
list.sort()     #sort the ascending order  [1, 2, 3]
list.sort(reverse=True)   #sorts in descending order [3, 2, 1]
list.reverse()  #reverse list  [3, 1, 2]
list.insert(idx, el)  #insert element at index -> Similer to the append, but its add values any particular idx
```

## List Methods
```python
list = [2, 1, 3, 1]
list.remove(1)  #remove first occurrence of element [2,3,1]
list.pop(idx)  #remove elemet at particular idx
```



