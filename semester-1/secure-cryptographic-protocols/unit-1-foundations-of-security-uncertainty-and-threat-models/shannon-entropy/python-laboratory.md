# 💻 Python Laboratory

### 📖 Overview

This laboratory introduces the practical implementation of **Shannon Entropy** using Python.

Instead of calculating entropy manually, we can develop Python programs that compute entropy for any probability distribution. This helps us verify numerical problems, analyze randomness, and understand how entropy behaves for different datasets.

By the end of this laboratory, you will be able to:

* Calculate Shannon Entropy using Python.
* Analyze different probability distributions.
* Compare entropy values.
* Visualize entropy.
* Apply entropy concepts to cybersecurity problems.

***

## 🧪 Experiment 1 – Shannon Entropy Calculator

### 🎯 Aim

To calculate the Shannon Entropy of a probability distribution.

***

### 📖 Theory

The Shannon Entropy formula is

$$
H(X)=-
\sum_{i=1}^{n}
P(x_i)\log_{2}(P(x_i))
$$

where

* $P(x\_i)$ = Probability of the $i^{th}$ outcome

***

### 💻 Python Program

```python
import math

probabilities = [0.5, 0.3, 0.2]

entropy = 0

for p in probabilities:
    entropy -= p * math.log2(p)

print("Entropy =", entropy, "bits")
```

***

### ✅ Output

```
Entropy = 1.4854752972273344 bits
```

***

### 📌 Observation

The calculated entropy matches the manual numerical solution.

***

## 🧪 Experiment 2 – Fair Coin Entropy

### 🎯 Aim

Calculate the entropy of a fair coin.

***

### 💻 Python Program

```python
import math

p = [0.5, 0.5]

entropy = -sum(i * math.log2(i) for i in p)

print(entropy)
```

***

### ✅ Output

```
1.0
```

***

### 📌 Observation

A fair coin has an entropy of **1 bit**, representing maximum uncertainty for two equally likely outcomes.

***

## 🧪 Experiment 3 – Biased Coin

### 🎯 Aim

Compare the entropy of a biased coin.

***

### 💻 Python Program

```python
import math

p = [0.9, 0.1]

entropy = -sum(i * math.log2(i) for i in p)

print(entropy)
```

***

### ✅ Output

```
0.4689955935892812
```

***

### 📌 Observation

The entropy is lower because one outcome is much more likely than the other.

***

## 🧪 Experiment 4 – User Input Entropy Calculator

### 🎯 Aim

Allow the user to enter any probability distribution.

***

### 💻 Python Program

```python
import math

n = int(input("Number of outcomes: "))

probabilities = []

for i in range(n):
    p = float(input(f"Enter probability {i+1}: "))
    probabilities.append(p)

entropy = 0

for p in probabilities:
    entropy -= p * math.log2(p)

print("\nShannon Entropy =", entropy, "bits")
```

***

### Example

```
Number of outcomes: 3

0.5
0.3
0.2
```

Output

```
Shannon Entropy = 1.485 bits
```

***

## 🧪 Experiment 5 – Password Entropy

### 🎯 Aim

Estimate the theoretical entropy of a password.

***

### 📖 Formula

$$
H=L\times\log_{2}(N)
$$

where

* $L$ = Password length
* $N$ = Character set size

***

### 💻 Python Program

```python
import math

length = int(input("Password Length: "))
charset = int(input("Character Set Size: "))

entropy = length * math.log2(charset)

print("Password Entropy =", round(entropy,2), "bits")
```

***

### Example

```
Length = 12

Charset = 94
```

Output

```
Password Entropy = 78.66 bits
```

***

## 🧪 Experiment 6 – Entropy Visualization

### 🎯 Aim

Visualize how entropy changes with probability.

***

### 💻 Python Program

```python
import numpy as np
import matplotlib.pyplot as plt

p = np.linspace(0.01,0.99,100)

entropy = -(p*np.log2(p)+(1-p)*np.log2(1-p))

plt.plot(p, entropy)

plt.xlabel("Probability")

plt.ylabel("Entropy")

plt.title("Binary Entropy Function")

plt.grid(True)

plt.show()
```

***

### 📌 Observation

The graph reaches its maximum at

$$
p=0.5
$$

which corresponds to maximum uncertainty.

***

## 🔐 Cybersecurity Applications

These Python programs can be used to:

* Evaluate password strength.
* Test random number generators.
* Verify entropy calculations.
* Compare probability distributions.
* Support cryptographic research.

***

## 🧪 Laboratory Exercises

1. Compute the entropy of a fair die.
2. Compare the entropy of two different password policies.
3. Modify the entropy calculator to ignore zero probabilities.
4. Plot entropy for probabilities from 0.01 to 0.99.
5. Compare a fair and biased coin using Python.

***

## 📝 Viva Questions

1. Why is entropy measured in bits?
2. Why do we use `math.log2()`?
3. Why is the negative sign required?
4. Why does entropy decrease for biased distributions?
5. What is the importance of entropy in cybersecurity?

***

## ⚠️ Common Errors

* Forgetting to import the **math** module.
* Using `log()` instead of `log2()`.
* Entering probabilities that do not sum to **1**.
* Including probability **0** in the logarithm calculation.
* Ignoring floating-point precision.

***

## 📌 Key Takeaways

* Python simplifies entropy calculations.
* Manual calculations can be verified programmatically.
* Entropy visualization improves conceptual understanding.
* Practical programming strengthens Information Theory concepts.

***

## 📝 Laboratory Summary

This laboratory demonstrated how Shannon Entropy can be implemented in Python to analyze uncertainty, verify numerical calculations, estimate password strength, and visualize entropy. These practical exercises reinforce the theoretical concepts introduced in the chapter and illustrate how entropy is applied in modern cryptography and cybersecurity.
