# 🔢 Data Types

## 🔢 Data Types

A **data type** defines the nature of data that a variable can store and determines the operations that can be performed on that data. Every value in Python belongs to a specific data type, and Python automatically determines the appropriate type when a value is assigned to a variable.

Python is a **dynamically typed** programming language, meaning programmers are not required to explicitly declare the type of a variable. Instead, the Python interpreter determines the data type during runtime based on the assigned value.

Understanding data types is essential because they influence memory allocation, data manipulation, program behavior, and performance.

***

## 🎯 Learning Objectives

After completing this chapter, you will be able to:

* Understand the concept of data types.
* Identify Python's built-in data types.
* Differentiate between mutable and immutable objects.
* Perform type conversion.
* Check the type of variables.
* Select appropriate data types for different applications.
* Apply data types in cybersecurity scenarios.

***

## 📖 What are Data Types?

A **data type** specifies:

* What kind of value is stored.
* How much memory is required.
* What operations are permitted.
* How Python interprets and processes the value.

Example:

```python
name = "Sachin"
age = 22
cgpa = 8.9
```

Python automatically assigns:

* `name` → String
* `age` → Integer
* `cgpa` → Float

***

## 📚 Classification of Python Data Types

Python provides several built-in data types.

| Category | Data Types                         |
| -------- | ---------------------------------- |
| Numeric  | `int`, `float`, `complex`          |
| Boolean  | `bool`                             |
| Text     | `str`                              |
| Sequence | `list`, `tuple`, `range`           |
| Mapping  | `dict`                             |
| Set      | `set`, `frozenset`                 |
| Binary   | `bytes`, `bytearray`, `memoryview` |
| Special  | `NoneType`                         |

***

## 🔢 Numeric Data Types

Numeric types store numerical values.

### Integer (`int`)

Stores whole numbers.

```python
age = 22
print(type(age))
```

Output

```
<class 'int'>
```

***

### Float (`float`)

Stores decimal numbers.

```python
cgpa = 8.75
print(type(cgpa))
```

Output

```
<class 'float'>
```

***

### Complex (`complex`)

Stores complex numbers.

```python
z = 4 + 5j
print(type(z))
```

Output

```
<class 'complex'>
```

***

## 🔤 String (`str`)

A string is an immutable sequence of Unicode characters.

```python
language = "Python"

print(type(language))
```

***

## 📋 List (`list`)

Lists are **ordered**, **mutable**, and allow duplicate elements.

```python
ports = [22, 80, 443]

print(type(ports))
```

***

## 📌 Tuple (`tuple`)

Tuples are **ordered**, **immutable**, and allow duplicate values.

```python
coordinates = (28.61, 77.20)

print(type(coordinates))
```

***

## 📖 Dictionary (`dict`)

Dictionaries store information as **key-value pairs**.

```python
student = {
    "name": "Sachin",
    "cgpa": 8.9
}
```

***

## 🎯 Set (`set`)

Sets store **unique** values.

```python
ports = {22,80,443}

print(type(ports))
```

***

## ✅ Boolean (`bool`)

Represents logical values.

```python
logged_in = True

print(type(logged_in))
```

***

## 🚫 NoneType

Represents the absence of a value.

```python
result = None

print(type(result))
```

Output

```
<class 'NoneType'>
```

***

## 🔄 Mutable vs Immutable Objects

One of the most important concepts in Python is object mutability.

### Mutable Objects

Can be modified after creation.

Examples:

* list
* dictionary
* set
* bytearray

Example

```python
numbers = [1,2,3]

numbers.append(4)
```

***

### Immutable Objects

Cannot be modified after creation.

Examples:

* int
* float
* bool
* tuple
* string
* frozenset

Example

```python
name = "Python"

name = name + "3"
```

Instead of modifying the original string, Python creates a new object.

***

## 📊 Mutable vs Immutable Comparison

| Mutable   | Immutable |
| --------- | --------- |
| list      | tuple     |
| dict      | string    |
| set       | int       |
| bytearray | float     |
|           | bool      |
|           | complex   |

***

## 🔍 Type Checking

Python provides built-in functions for checking data types.

### `type()`

```python
username = "admin"

print(type(username))
```

***

### `isinstance()`

```python
age = 22

print(isinstance(age, int))
```

Output

```
True
```

***

## 🔄 Type Conversion

Python allows explicit conversion between data types.

Common conversion functions:

| Function  | Description                              |
| --------- | ---------------------------------------- |
| `int()`   | Convert to integer                       |
| `float()` | Convert to float                         |
| `str()`   | Convert to string                        |
| `bool()`  | Convert to boolean                       |
| `list()`  | Convert to list                          |
| `tuple()` | Convert to tuple                         |
| `set()`   | Convert to set                           |
| `dict()`  | Convert to dictionary (where applicable) |

***

### Example

```python
age = "22"

print(int(age))

price = "99.95"

print(float(price))
```

***

## 💾 Memory Considerations

Every Python object occupies memory.

Immutable objects often improve safety and predictability because their values cannot change unexpectedly.

Mutable objects allow efficient updates but require careful handling when shared between variables.

Choosing the correct data type can improve both performance and code readability.

***

## 🌍 Real-World Example

```python
username = "admin"

failed_attempts = 4

allowed_ports = [22,80,443]

user_permissions = {
    "read": True,
    "write": False
}
```

Different data types are used together to represent application data.

***

## 🛡️ Cybersecurity Perspective

Data types are fundamental in cybersecurity programming.

Examples include:

| Data Type  | Cybersecurity Usage                  |
| ---------- | ------------------------------------ |
| String     | IP addresses, usernames, hashes      |
| Integer    | Port numbers, packet counts          |
| List       | Open ports, detected vulnerabilities |
| Dictionary | HTTP headers, JSON responses         |
| Set        | Unique IP addresses                  |
| Boolean    | Authentication status                |
| Bytes      | Network packets, encrypted data      |

Selecting the correct data type improves efficiency and simplifies data processing in security tools.

***

## 💡 Best Practices

* Choose the most appropriate data type.
* Use immutable objects when modification is unnecessary.
* Convert types only when required.
* Validate data before conversion.
* Keep related information grouped logically.

***

## ⚠️ Common Mistakes

* Confusing lists with tuples.
* Assuming strings are mutable.
* Performing calculations on strings without conversion.
* Using the wrong collection type.
* Ignoring mutability when modifying shared objects.

***

## 📌 Key Takeaways

* Every value in Python has a data type.
* Python automatically determines data types at runtime.
* Mutable and immutable objects behave differently.
* Type conversion enables flexible data processing.
* Proper data type selection improves readability, efficiency, and reliability.

***

## 📝 Summary

Data types form the foundation of every Python program by defining how information is stored, processed, and manipulated. Python provides a rich collection of built-in data types that support different categories of data, including numbers, text, collections, and binary information. Understanding mutability, type conversion, and appropriate data type selection is essential for writing efficient, maintainable, and secure Python applications, particularly in cybersecurity where different forms of structured and unstructured data are processed continuously.
