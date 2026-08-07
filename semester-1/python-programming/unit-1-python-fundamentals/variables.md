# 📊 Variables

## 📊 Variables

Variables are one of the fundamental building blocks of programming. A **variable** is a named reference to a memory location that stores a value. It allows a program to store, retrieve, and manipulate data during execution.

In Python, variables are created automatically when a value is assigned to them. Unlike statically typed programming languages such as C or Java, Python does **not require explicit declaration of variable types**. Instead, Python determines the data type automatically based on the assigned value, a feature known as **dynamic typing**.

Variables make programs flexible by allowing values to change during execution without modifying the program's logic.

***

## 🎯 Learning Objectives

After completing this chapter, you will be able to:

* Understand the concept of variables.
* Create and assign variables in Python.
* Explain dynamic typing.
* Understand how variables reference objects in memory.
* Perform multiple assignments and unpacking.
* Follow Python naming conventions.
* Apply variables in cybersecurity applications.

***

## 📖 What is a Variable?

A **variable** is an identifier that refers to a value stored in memory.

Think of a variable as a **label attached to an object** rather than a container that permanently holds data.

Example:

```python
name = "Sachin"

print(name)
```

Output

```
Sachin
```

Here:

* `name` is the variable.
* `"Sachin"` is the stored value.
* `=` is the assignment operator.

***

## 🧠 Variables and Memory

Unlike many programming languages, Python variables reference **objects** in memory.

```python
x = 10
y = x
```

Illustration:

```
Memory

+-------+
|  10   |
+-------+
   ▲
   │
+-----+     +-----+
|  x  |     |  y  |
+-----+     +-----+
```

Both `x` and `y` reference the same object until one of them is reassigned.

This model improves flexibility and simplifies memory management.

***

## ✍️ Creating Variables

Variables are created using the assignment operator (`=`).

Syntax

```python
variable_name = value
```

Example

```python
username = "admin"

age = 22

cgpa = 8.9

is_active = True
```

***

## 🔄 Dynamic Typing

Python automatically determines the type of a variable based on its assigned value.

```python
x = 100

print(type(x))

x = "Cyber Security"

print(type(x))
```

Output

```
<class 'int'>

<class 'str'>
```

The variable `x` changes from an integer to a string without requiring explicit type declarations.

***

## 📦 Multiple Assignment

Python allows multiple variables to be assigned values in a single statement.

```python
x, y, z = 10, 20, 30

print(x)

print(y)

print(z)
```

Output

```
10

20

30
```

***

## 🔁 Assigning the Same Value

A single value can be assigned to multiple variables.

```python
a = b = c = 100

print(a)

print(b)

print(c)
```

***

## 🎁 Variable Unpacking

Python can unpack values from sequences directly into variables.

```python
name, age, city = ("Sachin", 22, "Agra")

print(name)

print(age)

print(city)
```

Output

```
Sachin

22

Agra
```

***

## 🏷️ Variable Naming Rules

A variable name:

* Must begin with a letter (`A–Z` or `a–z`) or an underscore (`_`).
* May contain letters, digits, and underscores.
* Cannot begin with a digit.
* Cannot contain spaces.
* Cannot contain special characters (except `_`).
* Cannot use Python keywords.
* Is case-sensitive.

***

## 📐 Naming Conventions (PEP 8)

Python follows the **PEP 8 Style Guide** for naming variables.

| Variable Type    | Convention                   | Example        |
| ---------------- | ---------------------------- | -------------- |
| Variable         | `snake_case`                 | `student_name` |
| Constant         | `UPPER_CASE`                 | `MAX_USERS`    |
| Private Variable | `_single_leading_underscore` | `_token`       |

Good Examples

```python
student_name

total_marks

ip_address

failed_login_count
```

Poor Examples

```python
x

abc123

StudentName

Data1
```

Meaningful names improve readability and maintainability.

***

## 🔒 Constants

Python does not provide built-in constant variables.

By convention, variables that should not change are written using **uppercase letters**.

Example

```python
PI = 3.14159

MAX_CONNECTIONS = 100
```

Although these values can technically be modified, uppercase naming indicates that they should remain constant.

***

## 🔍 Checking Variable Types

The built-in `type()` function returns the data type of a variable.

```python
username = "admin"

print(type(username))
```

Output

```
<class 'str'>
```

***

## 🌍 Real-World Example

```python
username = "admin"

failed_login_attempts = 5

is_authenticated = False

ip_address = "192.168.1.100"
```

These variables might represent information used in a login monitoring or intrusion detection system.

***

## 🛡️ Cybersecurity Perspective

Variables are used extensively in cybersecurity applications to store and process information such as:

* Usernames
* IP addresses
* Network ports
* Hash values
* API tokens
* Security logs
* File paths
* Vulnerability scan results
* Threat intelligence indicators

> **Security Note:** Avoid storing sensitive information such as passwords, API keys, or cryptographic secrets in plain-text variables in production applications. Use secure storage mechanisms such as environment variables or dedicated secrets management systems.

***

## 💡 Best Practices

* Use meaningful variable names.
* Follow the `snake_case` naming convention.
* Keep variable names concise and descriptive.
* Use constants for fixed values.
* Avoid single-letter variable names except in simple loops.
* Initialize variables before use.
* Follow PEP 8 naming conventions.

***

## ⚠️ Common Mistakes

* Starting variable names with numbers.
* Using Python keywords as variable names.
* Choosing unclear or meaningless names.
* Assuming Python variables store values instead of referencing objects.
* Storing sensitive information directly in variables.

***

## 📌 Key Takeaways

* Variables are named references to objects in memory.
* Python uses dynamic typing.
* Variables are created automatically during assignment.
* Multiple assignment and unpacking simplify code.
* Meaningful naming improves readability.
* Variables are essential for storing and processing application data.

***

## 📝 Summary

Variables provide a mechanism for storing and manipulating data during program execution. Python's dynamic typing, object reference model, and flexible assignment syntax make variable management simple and efficient. By following proper naming conventions, understanding memory references, and applying secure coding practices, developers can create maintainable and reliable Python applications suitable for both general software development and cybersecurity automation.
