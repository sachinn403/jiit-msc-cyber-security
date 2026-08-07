# ⌨️ Input & Output Operations

## ⌨️ Input & Output (I/O) Operations

Input and Output (I/O) operations enable a program to communicate with users and external systems. **Input** refers to the process of receiving data, while **Output** refers to displaying or transmitting processed information.

Every interactive application relies on I/O operations. Whether collecting user credentials, reading configuration files, displaying analysis results, or generating security reports, Python provides simple yet powerful mechanisms for handling input and output.

Python primarily uses the built-in **`input()`** function for accepting user input and the **`print()`** function for displaying output.

***

## 🎯 Learning Objectives

After completing this chapter, you will be able to:

* Understand the concept of Input and Output.
* Accept user input using the `input()` function.
* Display formatted output using the `print()` function.
* Convert input into appropriate data types.
* Customize output formatting.
* Apply secure input handling techniques.
* Understand the importance of I/O in cybersecurity applications.

***

## 📖 What is Input?

**Input** is any data provided to a program during execution.

Input may come from:

* Keyboard
* Files
* Network
* Database
* APIs
* Sensors

In this chapter, we focus on **keyboard input**.

***

## 📖 What is Output?

**Output** is the information produced by a program after processing input.

Output may be displayed on:

* Terminal
* Console
* GUI
* File
* Network
* Log file

Python uses the `print()` function for console output.

***

## 📥 Receiving User Input

Python provides the **`input()`** function to receive data from the user.

### Syntax

```python
input("Prompt")
```

Example

```python
name = input("Enter your name: ")

print(name)
```

Output

```
Enter your name: Sachin

Sachin
```

***

## 📝 The `input()` Function Always Returns a String

One of the most important concepts in Python is that **`input()` always returns a string**, regardless of what the user enters.

Example

```python
age = input("Enter your age: ")

print(type(age))
```

Output

```
<class 'str'>
```

***

## 🔄 Type Conversion

To perform calculations, convert input into the required data type.

### Integer

```python
age = int(input("Enter Age: "))
```

***

### Float

```python
salary = float(input("Enter Salary: "))
```

***

### Boolean

```python
status = bool(input("Enter Status: "))
```

***

### String

```python
name = str(input("Enter Name: "))
```

***

## 📤 Displaying Output

Python uses the **`print()`** function to display information.

Syntax

```python
print(value)
```

Example

```python
print("Hello Python")
```

Output

```
Hello Python
```

***

## 🖨️ Printing Multiple Values

```python
name = "Sachin"

age = 22

print(name, age)
```

Output

```
Sachin 22
```

***

## 🎨 Formatted Output

Python supports several methods for formatting output.

***

### 1️⃣ f-Strings (Recommended)

Introduced in Python 3.6, f-strings provide a concise and readable way to embed variables directly into strings.

```python
name = "Sachin"

age = 22

print(f"My name is {name} and I am {age} years old.")
```

Output

```
My name is Sachin and I am 22 years old.
```

***

### 2️⃣ `format()` Method

```python
name = "Sachin"

print("Welcome {}".format(name))
```

***

### 3️⃣ `%` Formatting (Legacy)

```python
name = "Sachin"

print("Welcome %s" % name)
```

Although still supported, f-strings are preferred for modern Python development.

***

## ⚙️ The `sep` Parameter

The `sep` parameter specifies the separator between multiple values.

```python
print("Python", "Java", "Go", sep=" | ")
```

Output

```
Python | Java | Go
```

***

## ⚙️ The `end` Parameter

The `end` parameter controls what is printed after the output.

Default:

```python
print("Hello")
print("World")
```

Output

```
Hello
World
```

Custom:

```python
print("Hello", end=" ")
print("World")
```

Output

```
Hello World
```

***

## 📊 Standard Input, Output and Error Streams

Python programs interact with three standard streams.

| Stream                     | Purpose                 |
| -------------------------- | ----------------------- |
| Standard Input (`stdin`)   | Receives input          |
| Standard Output (`stdout`) | Displays normal output  |
| Standard Error (`stderr`)  | Displays error messages |

These streams form the basis of console applications and many automation scripts.

***

## 🌍 Real-World Example

```python
username = input("Username: ")

password = input("Password: ")

print(f"Welcome {username}")
```

Applications such as login systems, registration portals, and administrative tools rely heavily on user input and output.

***

## 🛡️ Cybersecurity Perspective

Input and Output operations are fundamental in cybersecurity applications.

Examples include:

* Reading usernames and passwords.
* Accepting IP addresses for network scanning.
* Processing command-line arguments.
* Displaying scan reports.
* Reading log files.
* Generating forensic reports.
* Displaying vulnerability assessment results.

> **Security Note:** Never trust user input. Always validate and sanitize data before processing it. Sensitive information such as passwords should not be displayed in plain text.

***

## 💡 Best Practices

* Always validate user input.
* Convert input into the required data type.
* Use meaningful prompt messages.
* Prefer f-strings for formatting.
* Keep output clear and user-friendly.
* Avoid exposing sensitive information.

***

## ⚠️ Common Mistakes

* Forgetting that `input()` returns a string.
* Performing arithmetic without type conversion.
* Displaying confidential information.
* Writing unclear prompt messages.
* Ignoring invalid input.

***

## 📌 Key Takeaways

* Input allows programs to receive data.
* Output allows programs to display information.
* `input()` always returns a string.
* Use type conversion for numerical calculations.
* f-strings are the recommended formatting technique.
* Secure handling of input is essential in cybersecurity.

***

## 📝 Summary

Input and Output operations enable communication between Python programs and users. The `input()` function collects information, while the `print()` function presents results. Understanding type conversion, output formatting, and secure input handling allows developers to build reliable, interactive, and secure applications. In cybersecurity, effective I/O operations are essential for automation, log processing, reporting, and user interaction.
