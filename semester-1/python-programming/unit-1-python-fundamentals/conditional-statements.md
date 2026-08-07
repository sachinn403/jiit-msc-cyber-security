# 🔀 Conditional Statements

## 🔀 Conditional Statements

Conditional statements are control flow structures that enable a program to make decisions based on specified conditions. Instead of executing every statement sequentially, a program can evaluate one or more conditions and execute different blocks of code depending on whether those conditions evaluate to **True** or **False**.

Decision-making is one of the most fundamental concepts in programming. In Python, conditional statements are implemented using the `if`, `elif`, and `else` keywords. These statements allow programs to respond dynamically to user input, system states, and runtime conditions.

Conditional statements are widely used in authentication systems, input validation, access control, business logic, cybersecurity automation, and intelligent decision-making applications.

***

## 🎯 Learning Objectives

After completing this chapter, you will be able to:

* Understand conditional execution.
* Use `if`, `elif`, and `else` statements.
* Write nested conditional statements.
* Evaluate Boolean expressions.
* Understand truthy and falsy values.
* Use conditional expressions effectively.
* Apply conditional logic in cybersecurity applications.

***

## 📖 What are Conditional Statements?

A conditional statement evaluates a condition and executes a block of code only when that condition is satisfied.

General Syntax

```python
if condition:
    # Code Block
```

If the condition evaluates to `True`, the code block executes. Otherwise, it is skipped.

***

## 🧠 Boolean Expressions

A condition in Python evaluates to either:

* `True`
* `False`

Example

```python
age = 20

print(age >= 18)
```

Output

```
True
```

Conditional statements rely on Boolean expressions to determine program flow.

***

## 1️⃣ The `if` Statement

The `if` statement executes a block of code only when the condition is true.

Syntax

```python
if condition:
    # Code
```

Example

```python
marks = 75

if marks >= 40:
    print("Pass")
```

Output

```
Pass
```

***

## 2️⃣ The `if...else` Statement

The `else` block executes when the `if` condition evaluates to `False`.

Syntax

```python
if condition:
    # Code
else:
    # Code
```

Example

```python
age = 16

if age >= 18:
    print("Eligible")
else:
    print("Not Eligible")
```

***

## 3️⃣ The `if...elif...else` Statement

When multiple conditions need to be evaluated, Python provides the `elif` keyword.

Syntax

```python
if condition1:
    # Code
elif condition2:
    # Code
else:
    # Code
```

Example

```python
marks = 82

if marks >= 90:
    print("Grade A+")
elif marks >= 75:
    print("Grade A")
elif marks >= 60:
    print("Grade B")
else:
    print("Grade C")
```

***

## 4️⃣ Nested Conditional Statements

An `if` statement can be placed inside another `if` statement.

Example

```python
age = 22
citizen = True

if age >= 18:
    if citizen:
        print("Eligible to Vote")
```

Nested conditions are useful when multiple levels of verification are required.

***

## ⚖️ Comparison Operators in Conditions

Conditional statements commonly use comparison operators.

| Operator | Meaning               |
| -------- | --------------------- |
| `==`     | Equal to              |
| `!=`     | Not Equal to          |
| `>`      | Greater Than          |
| `<`      | Less Than             |
| `>=`     | Greater Than or Equal |
| `<=`     | Less Than or Equal    |

Example

```python
salary = 50000

if salary >= 30000:
    print("Eligible")
```

***

## 🔗 Logical Operators in Conditions

Logical operators combine multiple conditions.

#### `and`

```python
age = 25

if age >= 18 and age <= 60:
    print("Eligible")
```

***

#### `or`

```python
day = "Sunday"

if day == "Saturday" or day == "Sunday":
    print("Weekend")
```

***

#### `not`

```python
logged_in = False

if not logged_in:
    print("Please Login")
```

***

## 💡 Truthy and Falsy Values

In Python, not every condition has to be explicitly `True` or `False`.

Some values are automatically treated as **False**.

Falsy values include:

```python
False
None
0
0.0
""
[]
{}
set()
```

Everything else is generally considered **Truthy**.

Example

```python
password = ""

if password:
    print("Password Entered")
else:
    print("Password Missing")
```

***

## ⚡ Conditional (Ternary) Expression

Python provides a concise syntax for simple conditional assignments.

Syntax

```python
value_if_true if condition else value_if_false
```

Example

```python
age = 20

status = "Adult" if age >= 18 else "Minor"

print(status)
```

Output

```
Adult
```

***

## 🌍 Real-World Example

```python
username = "admin"
password = "admin123"

if username == "admin" and password == "admin123":
    print("Access Granted")
else:
    print("Access Denied")
```

Conditional statements are the foundation of login systems and authentication mechanisms.

***

## 🛡️ Cybersecurity Perspective

Conditional logic is one of the most frequently used concepts in cybersecurity.

Examples include:

* User authentication
* Multi-factor authentication (MFA)
* Firewall rule evaluation
* Intrusion Detection System (IDS) alerts
* Password policy enforcement
* Role-Based Access Control (RBAC)
* Security policy enforcement
* Risk scoring and alert generation

Example:

```python
failed_attempts = 6

if failed_attempts >= 5:
    print("Account Locked")
else:
    print("Login Allowed")
```

***

## 💡 Best Practices

* Keep conditions simple and readable.
* Use meaningful variable names.
* Avoid deeply nested conditions.
* Use `elif` instead of multiple independent `if` statements where appropriate.
* Use parentheses to improve readability in complex logical expressions.
* Write conditions that clearly express the intended logic.

***

## ⚠️ Common Mistakes

* Using `=` instead of `==`.
* Incorrect indentation.
* Forgetting the colon (`:`).
* Writing overly complex nested conditions.
* Ignoring truthy and falsy behavior.
* Repeating the same condition unnecessarily.

***

## 📌 Key Takeaways

* Conditional statements control the flow of program execution.
* Python provides `if`, `elif`, and `else` for decision-making.
* Boolean expressions evaluate to `True` or `False`.
* Logical operators combine multiple conditions.
* Truthy and falsy values simplify conditional checks.
* Conditional logic is essential in cybersecurity applications such as authentication and access control.

***

## 📝 Summary

Conditional statements enable Python programs to make intelligent decisions by evaluating Boolean expressions and executing different code paths based on runtime conditions. Python's `if`, `elif`, and `else` constructs, combined with logical operators and comparison operators, provide a flexible framework for implementing decision-making logic. These concepts are indispensable in modern software development and play a central role in cybersecurity applications such as authentication, authorization, intrusion detection, and policy enforcement.
