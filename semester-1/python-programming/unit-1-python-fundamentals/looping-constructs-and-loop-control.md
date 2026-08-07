# 🔁 Looping Constructs & Loop Control

## 🔁 Looping Constructs & Loop Control

Loops are control flow structures that enable a program to execute a block of code repeatedly until a specified condition is met or until all elements in a sequence have been processed. Instead of writing the same statements multiple times, loops automate repetitive tasks, making programs shorter, more efficient, and easier to maintain.

In Python, two primary looping constructs are available:

* **`for` loop** – Used for iterating over sequences such as lists, tuples, dictionaries, strings, and ranges.
* **`while` loop** – Used when repetition depends on a condition rather than a fixed sequence.

Python also provides loop control statements such as `break`, `continue`, and `pass`, allowing developers to modify the normal execution of loops.

Loops are fundamental in automation, data processing, network programming, cybersecurity scripting, and software development.

***

## 🎯 Learning Objectives

After completing this chapter, you will be able to:

* Understand the purpose of loops.
* Differentiate between `for` and `while` loops.
* Use the `range()` function effectively.
* Control loop execution using `break`, `continue`, and `pass`.
* Understand nested loops.
* Use the optional `else` clause with loops.
* Apply loops to real-world cybersecurity automation tasks.

***

## 📖 Why Do We Need Loops?

Consider displaying the numbers from 1 to 5.

Without loops:

```python
print(1)
print(2)
print(3)
print(4)
print(5)
```

This approach becomes inefficient as the number of repetitions increases.

Using a loop:

```python
for number in range(1, 6):
    print(number)
```

Loops eliminate repetitive code, improve readability, and simplify maintenance.

***

## 🔄 The `for` Loop

The `for` loop is used to iterate over a sequence or iterable object.

### Syntax

```python
for variable in sequence:
    # Code Block
```

Example

```python
languages = ["Python", "Java", "C++"]

for language in languages:
    print(language)
```

Output

```
Python
Java
C++
```

***

## 🔢 The `range()` Function

The `range()` function generates a sequence of numbers and is commonly used with `for` loops.

#### `range(stop)`

```python
for i in range(5):
    print(i)
```

Output

```
0
1
2
3
4
```

***

#### `range(start, stop)`

```python
for i in range(1, 6):
    print(i)
```

Output

```
1
2
3
4
5
```

***

#### `range(start, stop, step)`

```python
for i in range(0, 10, 2):
    print(i)
```

Output

```
0
2
4
6
8
```

***

## 🔄 The `while` Loop

The `while` loop executes repeatedly as long as a condition evaluates to `True`.

### Syntax

```python
while condition:
    # Code Block
```

Example

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

Output

```
1
2
3
4
5
```

***

## ⛔ The `break` Statement

The `break` statement immediately terminates the loop.

Example

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

Output

```
0
1
2
3
4
```

***

## ⏭️ The `continue` Statement

The `continue` statement skips the current iteration and moves to the next one.

Example

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

Output

```
0
1
3
4
```

***

## ⏸️ The `pass` Statement

The `pass` statement performs no action. It acts as a placeholder where Python syntax requires a statement.

Example

```python
for i in range(5):
    if i == 3:
        pass
    print(i)
```

***

## 🔁 Nested Loops

A loop can be placed inside another loop.

Example

```python
for row in range(3):
    for column in range(2):
        print(row, column)
```

Output

```
0 0
0 1
1 0
1 1
2 0
2 1
```

Nested loops are useful for processing tables, matrices, and multidimensional data.

***

## 🔄 The `else` Clause with Loops

Python provides an optional `else` clause that executes only if the loop completes normally (without encountering a `break` statement).

Example

```python
for i in range(5):
    print(i)
else:
    print("Loop Completed")
```

Output

```
0
1
2
3
4
Loop Completed
```

If a `break` statement is executed, the `else` block is skipped.

***

## 🔍 Iterating Over Different Data Structures

### String

```python
for character in "Python":
    print(character)
```

***

### List

```python
numbers = [10, 20, 30]

for number in numbers:
    print(number)
```

***

### Dictionary

```python
student = {
    "name": "Sachin",
    "age": 22
}

for key, value in student.items():
    print(key, value)
```

***

### Set

```python
ports = {22, 80, 443}

for port in ports:
    print(port)
```

***

## 🌍 Real-World Example

```python
open_ports = [22, 80, 443]

for port in open_ports:
    print(f"Scanning Port {port}")
```

Loops enable repetitive processing without duplicating code.

***

## 🛡️ Cybersecurity Perspective

Loops are extensively used in cybersecurity automation.

Examples include:

* Scanning multiple IP addresses.
* Checking open network ports.
* Reading and analysing log files.
* Testing password dictionaries.
* Processing packet captures.
* Enumerating system users.
* Performing vulnerability scans.
* Monitoring security events.

Example:

```python
failed_attempts = [3, 5, 1, 8]

for attempts in failed_attempts:
    if attempts >= 5:
        print("Generate Security Alert")
```

Automation scripts used in penetration testing, SOC operations, and digital forensics rely heavily on loops.

***

## 💡 Best Practices

* Choose the appropriate loop for the problem.
* Avoid unnecessary nested loops.
* Ensure `while` loop conditions eventually become `False`.
* Use `break` and `continue` only when they improve readability.
* Keep loop bodies short and easy to understand.

***

## ⚠️ Common Mistakes

* Creating infinite `while` loops.
* Forgetting to update loop variables.
* Modifying a collection while iterating over it.
* Using nested loops unnecessarily.
* Misusing `break` and `continue`.

***

## 📌 Key Takeaways

* Loops automate repetitive tasks.
* Python provides `for` and `while` loops.
* The `range()` function generates numeric sequences.
* `break`, `continue`, and `pass` modify loop execution.
* Nested loops process multidimensional data.
* The optional `else` clause executes when a loop completes normally.
* Loops are fundamental to scripting and cybersecurity automation.

***

## 📝 Summary

Looping constructs provide an efficient mechanism for executing repetitive tasks while reducing code duplication. Python's `for` and `while` loops, combined with loop control statements such as `break`, `continue`, and `pass`, offer a flexible framework for iteration and automation. Features such as nested loops and the optional `else` clause further enhance Python's expressive power. These concepts form the foundation of automation scripts widely used in software development and cybersecurity for tasks such as network scanning, log analysis, vulnerability assessment, and incident response.
