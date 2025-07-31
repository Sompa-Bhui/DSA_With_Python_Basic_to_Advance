## ✅ The 7 Standard Types of Operators in Python

1. **Arithmetic Operators**  
   Used for basic mathematical operations like addition, subtraction, multiplication, etc.

2. **Assignment Operators**  
   Used to assign values to variables.

3. **Comparison (Relational) Operators**  
   Used to compare two values and return `True` or `False`.

4. **Logical Operators**  
   Used to combine conditional statements.

5. **Identity Operators**  
   Used to compare the memory location of two objects.

6. **Membership Operators**  
   Used to check if a value is a member of a sequence (like list, tuple, string, etc).

7. **Bitwise Operators**  
   Used to perform operations at the binary level.

### 🔢 1. Arithmetic Operators (Math wale)

Use for basic mathematical calculations. 

| Operator | Kaam (Meaning)     | Example   | Output |
|----------|--------------------|-----------|--------|
| `+`      | Add                | `5 + 2`   | `7`    |
| `-`      | Subtract           | `5 - 2`   | `3`    |
| `*`      | Multiply           | `5 * 2`   | `10`   |
| `/`      | Divide             | `5 / 2`   | `2.5`  |
| `//`     | Floor Divide       | `5 // 2`  | `2`    |
| `%`      | Modulus (Remainder)| `5 % 2`   | `1`    |
| `**`     | Power (Exponent)   | `5 ** 2`  | `25`   |

Differents between division and floor division :
* Divisio:- Give output in decimal.
* Floor Division:- GIve output in Integer.

---

### 📝 2. Assignment Operators (= and more)

Ye values ko variable me store karte hain.

| Operator | Meaning                | Example     | Same as         |
|----------|------------------------|-------------|------------------|
| `=`      | Assign value           | `x = 5`     | `x = 5`          |
| `+=`     | Add & assign           | `x += 3`    | `x = x + 3`      |
| `-=`     | Subtract & assign      | `x -= 2`    | `x = x - 2`      |
| `*=`     | Multiply & assign      | `x *= 4`    | `x = x * 4`      |
| `/=`     | Divide & assign        | `x /= 2`    | `x = x / 2`      |
| `//=`    | Floor divide & assign  | `x //= 2`   | `x = x // 2`     |
| `%=`     | Modulus & assign       | `x %= 2`    | `x = x % 2`      |
| `**=`    | Power & assign         | `x **= 2`   | `x = x ** 2`     |

---

### ⚖️ 3. Comparison Operators (True/False return karte hain)

Ye check karte hain do values barabar hain ya nahi, bade/chhote hain ya nahi.

| Operator | Meaning           | Example     | Output |
|----------|-------------------|-------------|--------|
| `==`     | Equal to          | `5 == 5`    | `True` |
| `!=`     | Not equal to      | `5 != 3`    | `True` |
| `>`      | Greater than      | `5 > 3`     | `True` |
| `<`      | Less than         | `5 < 3`     | `False`|
| `>=`     | Greater or Equal  | `5 >= 5`    | `True` |
| `<=`     | Less or Equal     | `5 <= 2`    | `False`|

---

### 🧠 4. Logical Operators (Conditions combine karte hain)

Ye multiple conditions ko AND/OR/NOT se check karte hain.

| Operator | Meaning               | Example                     | Output  |
|----------|------------------------|------------------------------|---------|
| `and`    | Both True              | `x > 3 and x < 10`           | `True`  |
| `or`     | At least one True      | `x < 3 or x > 10`            | `False` |
| `not`    | Opposite (negation)    | `not(x > 3 and x < 10)`      | `False` |

---

### 🆔 5. Identity Operators (`is`, `is not`)

Ye check karte hain ki do variables ek hi object ko point kar rahe hain ya nahi.
* is (Returns True if both variables are the same object)
* id not (Returns True if both variables are not the same objects)

```python
a = [1, 2]
b = a
c = [1, 2]

a is b      # True  (same object)

---
```
### 🔍 6. Membership Operators (`in`, `not in`)

The membership operators in python are used to test whether a Value is found within a sequence or not.
* IN: True if value/variable is found the sequence.
```python
Eg: x = [1,2,3,4,5,6]
print(5 in x)
output : True
```

```python
"a" in "apple"       # True
"z" in "apple"       # False
3 in [1, 2, 3, 4]    # True
5 not in [1, 2, 3]   # True
```

---

### 🔍 6. Membership Operators (`in`, `not in`)

Ye check karte hain ki value kisi list, string, etc. me hai ya nahi.

```python
"a" in "apple"       # True
"z" in "apple"       # False
3 in [1, 2, 3, 4]    # True
5 not in [1, 2, 3]   # True
```
---

### ⚙️ 7. Bitwise Operators (Binary bits par kaam karte hain)

Computer ke `0s` and `1s` par directly operation karte hain.

Assume: `x = 5` (`0101`), `y = 3` (`0011`)

| Operator | Name        | Example     | Result (in binary)              |
|----------|-------------|-------------|---------------------------------|
| `&`      | AND         | `x & y`     | `1`  (`0101 & 0011 = 0001`)     |
| `|`      | OR          | `x | y`     | `7`  (`0101 | 0011 = 0111`)     |
| `^`      | XOR         | `x ^ y`     | `6`  (`0101 ^ 0011 = 0110`)     |
| `~`      | NOT         | `~x`        | `-6` (flips all bits of 5)      |
| `<<`     | Left shift  | `x << 1`    | `10` (shift bits left: `1010`)  |
| `>>`     | Right shift | `x >> 1`    | `2`  (shift bits right: `0010`) |

---

📌 Final Summary (Ek Line mein):
Type	Use for
* Arithmetic	Math operations
* Assignment	Values assign karne ke liye
* Comparison	Compare karne ke liye
* Logical	Conditions combine karne ke liye
* Identity	Object identity check
* Membership	List/String me value check
* Bitwise	Binary level operations



