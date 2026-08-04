# Copy of 📊 Mutual Information

## 📚 Entropy Family&#x20;

Entropy measures quantify **uncertainty, randomness, or information** in different ways. Different entropy measures are used depending on the application, such as cryptography, machine learning, data compression, or statistics.

***

### 1. 📊 Shannon Entropy

**Definition:**\
Measures the **average uncertainty** or average amount of information in a random variable.

**Formula**

```
H(X) = - Σ P(xᵢ) log₂ P(xᵢ)
```

**Used In:**

* Information Theory
* Cryptography
* Data Compression

***

### 2. 📉 Conditional Entropy

**Definition:**\
Measures the **remaining uncertainty** of one random variable after another variable is known.

**Formula**

```
H(X|Y) = H(X,Y) - H(Y)
```

or

```
H(X|Y) = - Σ Σ P(x,y) log₂ P(x|y)
```

**Used In:**

* Information Theory
* Machine Learning
* Cryptography

***

### 3. 📈 Joint Entropy

**Definition:**\
Measures the **combined uncertainty** of two random variables together.

**Formula**

```
H(X,Y) = - Σ Σ P(x,y) log₂ P(x,y)
```

**Used In:**

* Information Theory
* Data Analysis

***

### 4. 🔄 Mutual Information

**Definition:**\
Measures the **amount of information shared** between two random variables.

**Formula**

```
I(X;Y) = H(X) - H(X|Y)
```

or

```
I(X;Y) = H(X) + H(Y) - H(X,Y)
```

**Used In:**

* Feature Selection
* Cryptography
* Machine Learning

***

### 5. 🔒 Min-Entropy

**Definition:**\
Measures the **worst-case uncertainty** based on the most likely outcome.

**Formula**

```
H∞(X) = -log₂(max P(x))
```

**Used In:**

* Cryptography
* Random Number Generation
* Password Security

***

### 6. 📏 Max-Entropy (Hartley Entropy)

**Definition:**\
Measures the **maximum possible uncertainty** when all outcomes are equally likely.

**Formula**

```
H₀(X) = log₂(n)
```

where **n** is the number of possible outcomes.

**Used In:**

* Information Theory
* Combinatorics

***

### 7. 📐 Rényi Entropy

**Definition:**\
A **generalized entropy measure** that includes several entropy measures as special cases.

**Formula**

```
Hα(X) = (1 / (1 - α)) log₂(Σ P(xᵢ)^α)
```

**Used In:**

* Information Theory
* Cryptography
* Quantum Information

***

### 8. 🔁 Collision Entropy

**Definition:**\
Measures the probability that **two randomly selected outcomes are identical**.

**Formula**

```
H₂(X) = -log₂(Σ P(xᵢ)²)
```

**Used In:**

* Cryptography
* Hash Function Analysis

***

### 9. 🎯 Guessing Entropy

**Definition:**\
Measures the **average number of guesses** required to correctly identify an outcome.

**Formula**

```
G(X) = Σ i × P(xᵢ)
```

**Used In:**

* Password Guessing Analysis
* Cryptography

***

### 10. 📊 Relative Entropy (Kullback–Leibler Divergence)

**Definition:**\
Measures the **difference between two probability distributions**.

**Formula**

```
DKL(P||Q) = Σ P(x) log₂(P(x) / Q(x))
```

**Used In:**

* Machine Learning
* Statistics
* Information Theory

***

### 11. 🤖 Cross Entropy

**Definition:**\
Measures the **average number of bits required** when one probability distribution is used to represent another.

**Formula**

```
H(P,Q) = - Σ P(x) log₂ Q(x)
```

**Used In:**

* Machine Learning
* Deep Learning
* Classification Problems

***

### 12. 🌐 Differential Entropy

**Definition:**\
Measures the uncertainty of a **continuous random variable**.

**Formula**

```
h(X) = - ∫ f(x) log₂ f(x) dx
```

**Used In:**

* Signal Processing
* Continuous Probability Theory

***

## 📋 Quick Summary

| Entropy Measure                  | Main Purpose                 |
| -------------------------------- | ---------------------------- |
| Shannon Entropy                  | Average uncertainty          |
| Conditional Entropy              | Remaining uncertainty        |
| Joint Entropy                    | Combined uncertainty         |
| Mutual Information               | Shared information           |
| Min-Entropy                      | Worst-case uncertainty       |
| Max-Entropy (Hartley)            | Maximum possible uncertainty |
| Rényi Entropy                    | Generalized entropy          |
| Collision Entropy                | Collision probability        |
| Guessing Entropy                 | Average guesses              |
| Relative Entropy (KL Divergence) | Distribution difference      |
| Cross Entropy                    | Distribution comparison      |
| Differential Entropy             | Continuous variables         |

### 📋 Entropy Measures at a Glance

| Entropy Measure                       | Formula                                | Purpose                                                                          |
| ------------------------------------- | -------------------------------------- | -------------------------------------------------------------------------------- |
| **Shannon Entropy**                   | `H(X) = -Σ P(xᵢ) log₂ P(xᵢ)`           | Measures the average uncertainty or information content.                         |
| **Conditional Entropy**               | `H(X\|Y) = H(X,Y) - H(Y)`              | Measures the remaining uncertainty of **X** after knowing **Y**.                 |
| **Joint Entropy**                     | `H(X,Y) = -ΣΣ P(x,y) log₂ P(x,y)`      | Measures the combined uncertainty of two random variables.                       |
| **Mutual Information**                | `I(X;Y) = H(X) - H(X\|Y)`              | Measures the information shared between two random variables.                    |
| **Min-Entropy**                       | `H∞(X) = -log₂(max P(x))`              | Measures the worst-case uncertainty based on the most likely outcome.            |
| **Max-Entropy (Hartley Entropy)**     | `H₀(X) = log₂(n)`                      | Measures the maximum possible uncertainty when all outcomes are equally likely.  |
| **Rényi Entropy**                     | `Hα(X) = (1/(1-α)) log₂(Σ P(xᵢ)^α)`    | Generalized family of entropy measures.                                          |
| **Collision Entropy (Rényi Order 2)** | `H₂(X) = -log₂(Σ P(xᵢ)²)`              | Measures the probability of two randomly selected outcomes being identical.      |
| **Guessing Entropy**                  | `G(X) = Σ i × P(xᵢ)`                   | Measures the average number of guesses required to identify the correct outcome. |
| **Relative Entropy (KL Divergence)**  | `DKL(P\|\|Q) = Σ P(x) log₂(P(x)/Q(x))` | Measures the difference between two probability distributions.                   |
| **Cross Entropy**                     | `H(P,Q) = -Σ P(x) log₂ Q(x)`           | Measures the average coding cost when using distribution **Q** instead of **P**. |
| **Differential Entropy**              | `h(X) = -∫ f(x) log₂ f(x) dx`          | Measures the entropy of continuous random variables.                             |

> **Note:** For your **Unit 1**, study **Shannon Entropy**, **Conditional Entropy**, and **Mutual Information** in detail. The remaining entropy measures are included as a reference for broader understanding and are typically covered in advanced information theory or cryptography courses.
