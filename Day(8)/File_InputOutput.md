# Python File I/O Summary
File I/O is the process of **reading data from a file (input)** or **writing data to a file (output)** in Python.

# File I/O (Input/Output) in Python

File I/O is the process of **reading data from a file (input)** or **writing data to a file (output)** using Python.

## Input
Reading data from a file → `read()`

## Output
Writing data to a file → `write()`

Python provides the built-in `open()` function to work with files.

## 2. Opening a File

**Syntax:**  

```python
file = open("filename.txt", "mode")
```

# File I/O Modes in Python

| Character | Meaning                                                  |
|-----------|----------------------------------------------------------|
| 'r'       | Open for reading (default)                               |
| 'w'       | Open for writing, truncating the file first             |
| 'x'       | Create a new file and open it for writing               |
| 'a'       | Open for writing, appending to the end of the file if it exists |
| 'b'       | Binary mode                                              |
| 't'       | Text mode (default)                                     |
| '+'       | Open a disk file for updating (reading and writing)     |

## 3. Reading from a File

```python
file = open("example.txt", "r")  # Open in read mode
content = file.read()            # Read entire file
print(content)
file.close()                     # Close the file
```

## Other Reading Methods

```python
file = open("example.txt", "r")
print(file.readline())   # Read one line
print(file.readlines())  # Read all lines as a list
file.close()             # Close the file
```

## 4. Writing to a File

```python
file = open("example.txt", "w")  # Open in write mode
file.write("Hello, Python!\n")
file.write("This is a new line.")
file.close()                     # Close the file
```
## Append Mode

```python
file = open("example.txt", "a")  # Open in append mode
file.write("\nThis line will be added at the end.")
file.close()                      # Close the file
```

## 5. Using `with` Statement (Best Practice)

Automatically closes the file even if an error occurs.

```python
# Reading a file safely
with open("example.txt", "r") as file:
    content = file.read()
    print(content)

# Appending to a file safely
with open("example.txt", "a") as file:
    file.write("\nAdding another line safely.")
```

## 6. Working with Binary Files

```python
# Writing binary data
with open("data.bin", "wb") as file:
    file.write(b"Hello Binary")

# Reading binary data
with open("data.bin", "rb") as file:
    content = file.read()
    print(content)  # Output: b'Hello Binary'
```

## 7. File Methods (Important)

| Method             | Description                     |
|-------------------|---------------------------------|
| `file.read(n)`     | Reads `n` characters.           |
| `file.readline()`  | Reads one line.                 |
| `file.readlines()` | Reads all lines as a list.      |
| `file.write(string)` | Writes `string` to the file. |
| `file.seek(pos)`   | Move cursor to position `pos`.  |
| `file.tell()`      | Returns current cursor position.|
| `file.close()`     | Closes the file.                |

## Advanced Concepts

### Binary Files
Use `'rb'` for reading and `'wb'` for writing binary data.

### JSON Files
Use `json.dump()` to write JSON data and `json.load()` to read JSON data.

### Pickle Files
Use `pickle.dump()` to serialize Python objects and `pickle.load()` to deserialize them.

### Large Files
Read large files line by line to avoid memory issues.

### File Operations
- `os.path.exists()` → Check if a file exists  
- `shutil.copy()` → Copy a file  
- `file.seek()` → Move the cursor to a specific position  
- `file.tell()` → Get the current cursor position

## Key Points

- Always close files (or use `with` statement for automatic closing).

### Recap of Memory Efficiency
- **Small files** → `read()` is fine  
- **Large files** → loop line by line

### Binary vs Text Files
- **Binary files** → For images, objects, and non-text data  
- **Text files** → For strings and human-readable data


# Summary:-
Python can be used to perform operations on a file. (read & write data)

## Types of all files
There are basically two types of files.
### 1) Text Files: Data stores here in form of characters.
.txt, .docx, .log etc.

### 2) Binary Files
Data not stored in character form, e.g., `.mp4`, `.mov`, `.png`, `.jpeg`, etc.

## Open, Read & Close File
We have to open a file before reading or writing.

```python
f = open("file_name", "mode")  # Open file

# file name examples: "sample.txt" or "demo.docx"
# mode examples: 'r' for read, 'w' for write

data = f.read()  # Read data from file
f.close()        # Close the file
```


## Reading a file

with open("example.txt", "r") as f:
    data = f.read()        # reads entire file
    print(data)
```python
    dat = f.readline()     # reads one line at a time
    print(dat)
```
