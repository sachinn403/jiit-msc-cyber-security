# 📊 Shannon Entropy

## 📖 Overview

**Shannon Entropy** is a fundamental concept in information theory introduced by **Claude Shannon** in 1948. It measures the **uncertainty**, **randomness**, or **amount of information** in a random variable. In cryptography, higher entropy indicates greater unpredictability, making it more difficult for an attacker to guess or infer secret information.

***

### 🎯 Why is it Important?

* Measures the uncertainty of information.
* Forms the mathematical foundation of information theory.
* Helps evaluate the strength of cryptographic systems.
* Used in password security and key generation.
* Supports the analysis of secure communication protocols.

***

### 🔑 Key Concepts

#### 1. Entropy

Entropy is the average amount of information produced by a random event.

* High entropy → High uncertainty → Better security
* Low entropy → Low uncertainty → Easier to predict

***

#### 2. Random Variable

A **random variable (X)** represents the possible outcomes of an event.

**Example:**

```
X = {A, B, C}
```

***

#### 3. Probability Distribution

Each outcome has a probability.

**Example:**

| Outcome | Probability |
| ------- | ----------: |
| A       |         0.5 |
| B       |         0.3 |
| C       |         0.2 |

The probabilities must satisfy:

* 0 ≤ P(x) ≤ 1
* P(A) + P(B) + P(C) = 1

***

### 📐 Formula

H(X) = − Σᵢ₌₁ⁿ P(xᵢ) × log₂(P(xᵢ))

#### Where

* H(X) = Shannon Entropy
* P(xᵢ) = Probability of the iᵗʰ outcome
* Σ = Summation (add all outcomes)
* log₂ = Logarithm to base 2
* n = Number of possible outcomes

***

### 🧠 Interpretation

| Entropy Value | Meaning                         |
| ------------- | ------------------------------- |
| High          | More randomness and uncertainty |
| Low           | More predictability             |
| Zero          | Outcome is certain              |

***

### 📈 Properties of Shannon Entropy

* Entropy is always **non-negative**.
* Maximum entropy occurs when all outcomes are **equally likely**.
* Entropy is **0** if one outcome has probability **1**.
* Measured in **bits** when using **log₂**.
* Increases as uncertainty increases.

***

### 🌍 Real-World Examples

#### Example 1: Fair Coin

```
Head = 0.5
Tail = 0.5
```

Both outcomes are equally likely, so the uncertainty is high.

***

#### Example 2: Biased Coin

```
Head = 0.95
Tail = 0.05
```

Since one outcome is much more likely, the uncertainty is lower.

***

#### Example 3: Password Selection

If users choose passwords randomly from many possibilities, entropy is high.

If most users choose **123456** or **password**, entropy is low, making passwords easier to guess.

***

### 🧮 Solved Numerical 1 – Fair Coin

#### Given

* P(H) = 0.5
* P(T) = 0.5

#### Formula

H(X) = −Σ P(x) log₂ P(x)

#### Solution

H(X)

\= −\[(0.5 × log₂0.5) + (0.5 × log₂0.5)]

Since,

log₂0.5 = −1

Therefore,

\= −\[(0.5 × −1) + (0.5 × −1)]

\= −(−0.5 − 0.5)

\= 1 bit

#### Answer

**Entropy = 1 bit**

***

### 🧮 Solved Numerical 2 – Three Equal Outcomes

#### Given

* P(A) = 1/3
* P(B) = 1/3
* P(C) = 1/3

#### Formula

H(X) = −Σ P(x) log₂ P(x)

#### Solution

H(X)

\= −\[(1/3 × log₂(1/3))

* (1/3 × log₂(1/3))
* (1/3 × log₂(1/3))]

Since all three terms are equal,

\= −3 × (1/3 × log₂(1/3))

\= −log₂(1/3)

\= log₂3

≈ 1.585 bits

#### Answer

**Entropy ≈ 1.585 bits**

***

### 🧮 Solved Numerical 3 – Unequal Probabilities

#### Given

* P(A) = 0.5
* P(B) = 0.3
* P(C) = 0.2

#### Formula

H(X) = −Σ P(x) log₂ P(x)

#### Solution

H(X)

\= −\[(0.5 × log₂0.5)

* (0.3 × log₂0.3)
* (0.2 × log₂0.2)]

Using,

log₂0.5 = −1

log₂0.3 ≈ −1.737

log₂0.2 ≈ −2.322

Substituting,

\= −\[(0.5 × −1)

* (0.3 × −1.737)
* (0.2 × −2.322)]

\= −\[−0.5 −0.5211 −0.4644]

\= 1.4855 bits

≈ 1.485 bits

#### Answer

**Entropy ≈ 1.485 bits**

***

### 💡 Practice Questions

1. Calculate the entropy for:
   * P(A)=0.25
   * P(B)=0.25
   * P(C)=0.25
   * P(D)=0.25
2. Calculate the entropy for:
   * P(A)=0.7
   * P(B)=0.2
   * P(C)=0.1
3. A die has six equally likely outcomes. Find its entropy.
4. Which distribution has the highest entropy?
   * (0.5, 0.5)
   * (0.9, 0.1)
   * (1/3, 1/3, 1/3)

***

### ⚠️ Common Mistakes

* Forgetting the negative sign (−).
* Using probabilities that do not sum to **1**.
* Using the wrong logarithm base.
* Rounding intermediate values too early.
* Confusing **Shannon Entropy** with **Password Entropy**.

***

### 📌 Key Takeaways

* Shannon Entropy measures the uncertainty or randomness of information.
* Greater entropy means greater unpredictability and stronger security.
* Equal probability distributions produce the highest entropy.
* Entropy is measured in **bits** when using base-2 logarithms.
* Shannon Entropy is the foundation for concepts such as **Conditional Entropy**, **Mutual Information**, and **Perfect Secrecy**.
