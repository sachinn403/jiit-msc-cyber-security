# ➕ Operators & Expressions

## ➕ Operators & Expressions

Operators are special symbols used to perform operations on variables and values. An **expression** is a combination of variables, constants, operators, and function calls that evaluates to a single value.

Operators are essential for performing arithmetic calculations, comparisons, logical operations, data manipulation, and decision-making in Python programs.

***

## 🎯 Why are Operators Important?

Operators allow programmers to:

* Perform mathematical calculations.
* Compare values.
* Make decisions in programs.
* Manipulate variables.
* Combine logical conditions.
* Write efficient and readable code.

***

## 📚 Types of Operators in Python

Python provides the following categories of operators:

| Operator Type        | Description                         |
| -------------------- | ----------------------------------- |
| Arithmetic Operators | Perform mathematical operations     |
| Assignment Operators | Assign values to variables          |
| Comparison Operators | Compare two values                  |
| Logical Operators    | Combine multiple conditions         |
| Bitwise Operators    | Perform operations on binary values |
| Membership Operators | Check membership in a sequence      |
| Identity Operators   | Compare object identities           |

***

## 1️⃣ Arithmetic Operators

Arithmetic operators are used to perform mathematical calculations.

| Operator | Description    | Example  |
| -------- | -------------- | -------- |
| `+`      | Addition       | `5 + 2`  |
| `-`      | Subtraction    | `5 - 2`  |
| `*`      | Multiplication | `5 * 2`  |
| `/`      | Division       | `5 / 2`  |
| `//`     | Floor Division | `5 // 2` |
| `%`      | Modulus        | `5 % 2`  |
| `**`     | Exponentiation | `5 ** 2` |

#### Example

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

***

## 2️⃣ Assignment Operators

Assignment operators assign values to variables.

| Operator | Example   | Equivalent To |
| -------- | --------- | ------------- |
| `=`      | `x = 5`   | Assign value  |
| `+=`     | `x += 2`  | `x = x + 2`   |
| `-=`     | `x -= 2`  | `x = x - 2`   |
| `*=`     | `x *= 2`  | `x = x * 2`   |
| `/=`     | `x /= 2`  | `x = x / 2`   |
| `%=`     | `x %= 2`  | `x = x % 2`   |
| `//=`    | `x //= 2` | `x = x // 2`  |
| `**=`    | `x **= 2` | `x = x ** 2`  |

***

## 3️⃣ Comparison Operators

Comparison operators compare two values and return either `True` or `False`.

| Operator | Meaning                  |
| -------- | ------------------------ |
| `==`     | Equal to                 |
| `!=`     | Not equal to             |
| `>`      | Greater than             |
| `<`      | Less than                |
| `>=`     | Greater than or equal to |
| `<=`     | Less than or equal to    |

#### Example

```python
a = 10
b = 20

print(a == b)
print(a != b)
print(a < b)
print(a > b)
```

***

## 4️⃣ Logical Operators

Logical operators combine multiple conditions.

| Operator | Description                            |
| -------- | -------------------------------------- |
| `and`    | True if both conditions are true       |
| `or`     | True if at least one condition is true |
| `not`    | Reverses the result                    |

#### Example

```python
age = 20

print(age >= 18 and age <= 60)
print(age < 18 or age > 60)
print(not(age > 18))
```

***

## 5️⃣ Bitwise Operators

Bitwise operators work directly on binary values.

| Operator | Description |
| -------- | ----------- |
| `&`      | AND         |
| \`       | \`          |
| `^`      | XOR         |
| `~`      | NOT         |
| `<<`     | Left Shift  |
| `>>`     | Right Shift |

#### Example

```python
a = 5
b = 3

print(a & b)
print(a | b)
print(a ^ b)
```

***

## 6️⃣ Membership Operators

Membership operators check whether a value exists in a sequence.

| Operator | Description          |
| -------- | -------------------- |
| `in`     | Value exists         |
| `not in` | Value does not exist |

#### Example

```python
languages = ["Python", "Java", "C++"]

print("Python" in languages)
print("Go" not in languages)
```

***

## 7️⃣ Identity Operators

Identity operators compare whether two variables refer to the same object in memory.

| Operator | Description       |
| -------- | ----------------- |
| `is`     | Same object       |
| `is not` | Different objects |

#### Example

```python
x = [1, 2]
y = x
z = [1, 2]

print(x is y)
print(x is z)
print(x is not z)
```

***

## 🧮 Expressions

An expression is any valid combination of values, variables, operators, and function calls that produces a result.

#### Arithmetic Expression

```python
total = 50 + 25 * 2
```

#### Logical Expression

```python
age >= 18 and age <= 60
```

#### Comparison Expression

```python
marks > 40
```

***

## ⭐ Operator Precedence

When multiple operators are used in an expression, Python evaluates them according to precedence.

| Priority | Operators            |
| -------- | -------------------- |
| Highest  | `()` Parentheses     |
|          | `**` Exponentiation  |
|          | `*`, `/`, `//`, `%`  |
|          | `+`, `-`             |
|          | Comparison Operators |
|          | `not`                |
|          | `and`                |
| Lowest   | `or`                 |

#### Example

```python
result = 10 + 5 * 2

print(result)
```

Output

```
20
```

***

## 🌍 Real-World Example

```python
username = "admin"
password = "admin123"

if username == "admin" and password == "admin123":
    print("Login Successful")
else:
    print("Access Denied")
```

Operators are widely used in authentication systems, validation checks, and decision-making processes.

***

## ⭐ Best Practices

* Use parentheses to improve readability.
* Avoid overly complex expressions.
* Use comparison and logical operators carefully.
* Write clear and meaningful conditions.
* Follow Python's operator precedence rules.

***

## ⚠️ Common Mistakes

* Confusing `=` (assignment) with `==` (comparison).
* Using `is` instead of `==` for value comparison.
* Forgetting operator precedence.
* Writing overly complicated expressions.
* Misusing logical operators.

***

## 📌 Summary

Operators are fundamental building blocks in Python that perform calculations, comparisons, logical operations, and data manipulation. Expressions combine operators, variables, and values to produce results. Understanding the different types of operators and their precedence is essential for writing efficient, readable, and error-free Python programs.

> **Tip:** Use parentheses `()` whenever an expression becomes complex. This improves readability and ensures the intended order of evaluation.
