# 📈 Properties & Interpretation

### 📖 Overview

After deriving the Shannon Entropy formula, the next step is to understand what the entropy value actually represents.

Entropy is more than just a mathematical quantity—it provides insight into the **uncertainty**, **randomness**, and **predictability** of a random source. By studying its properties, we can determine when uncertainty is maximized, when it becomes zero, and how probability distributions influence the amount of information generated.

Understanding these properties is essential for analyzing secure cryptographic systems, password strength, and information leakage.

***

### 🎯 Why Study Entropy Properties?

The properties of Shannon Entropy help us to:

* Interpret entropy values correctly.
* Compare different probability distributions.
* Determine when uncertainty is maximum or minimum.
* Analyze randomness in cryptographic systems.
* Understand the relationship between probability and security.
* Build intuition before studying Conditional Entropy and Mutual Information.

***

### 🧠 Interpretation of Shannon Entropy

Entropy measures the **average uncertainty** before observing the outcome of a random event.

It answers the question:

> **"How uncertain are we before the event occurs?"**

* **High Entropy** → High uncertainty → Difficult to predict.
* **Low Entropy** → Low uncertainty → Easy to predict.

Entropy therefore measures **unpredictability**, not the meaning or importance of information.

***

### 📌 Properties of Shannon Entropy

#### 1. Entropy is Always Non-Negative

Entropy can never be negative.

$$
H(X)\ge0
$$

Reason:

* Probabilities are always between 0 and 1.
* The logarithm of a probability is negative.
* The negative sign in the entropy formula makes the final result non-negative.

***

#### 2. Entropy is Zero for a Certain Event

If an event is certain,

$$
P(x)=1
$$

then

$$
H(X)=0
$$

There is no uncertainty because the outcome is already known.

**Example**

The sun rises tomorrow.

Since the outcome is almost certain, almost no new information is gained.

***

#### 3. Maximum Entropy Occurs for Uniform Distributions

Entropy reaches its maximum value when all outcomes are equally likely.

Example:

Fair Coin

| Outcome | Probability |
| ------- | ----------: |
| Head    |         0.5 |
| Tail    |         0.5 |

No outcome is favored, so uncertainty is greatest.

***

#### 4. Entropy Decreases as Predictability Increases

If one outcome becomes much more likely than the others, entropy decreases.

Example:

| Outcome | Probability |
| ------- | ----------: |
| A       |        0.90 |
| B       |        0.10 |

Since outcome A is highly predictable, uncertainty is low.

***

#### 5. Entropy Depends Only on Probability Distribution

Entropy depends only on the probabilities of the outcomes.

It does **not** depend on:

* The names of the outcomes.
* The order of the outcomes.
* The meaning of the messages.

Only the probability distribution matters.

***

### 📈 Maximum Entropy

For a system with **n equally likely outcomes**,

$$
P(x)=\frac{1}{n}
$$

The maximum entropy is

$$
H_{\max}=\log_2 n
$$

#### Example

For a fair six-sided die,

$$
H=\log_2 6\approx2.585\text{ bits}
$$

***

### 📉 Minimum Entropy

Minimum entropy occurs when one outcome has probability 1.

Example:

| Outcome | Probability |
| ------- | ----------: |
| A       |         1.0 |
| B       |         0.0 |
| C       |         0.0 |

Since the outcome is already known,

$$
H=0
$$

***

### ⚖️ Uniform vs Non-Uniform Distribution

#### Uniform Distribution

* Equal probabilities.
* Maximum uncertainty.
* Maximum entropy.

Example:

| Outcome | Probability |
| ------- | ----------: |
| A       |        0.25 |
| B       |        0.25 |
| C       |        0.25 |
| D       |        0.25 |

***

#### Non-Uniform Distribution

* Unequal probabilities.
* Lower uncertainty.
* Lower entropy.

Example:

| Outcome | Probability |
| ------- | ----------: |
| A       |        0.70 |
| B       |        0.20 |
| C       |        0.10 |

***

### 🎯 Binary Entropy Function

For a binary random variable,

$$
H(p)=
-p\log_2(p)
-(1-p)\log_2(1-p)
$$

where:

* $$p$$ = Probability of one outcome.
* $$(1-p)$$ = Probability of the other outcome.

#### Important Observations

* Maximum entropy occurs at

$$
p=0.5
$$

* Minimum entropy occurs at

$$
p=0
\quad\text{or}\quad
p=1
$$

***

### 🔄 Relationship Between Probability and Entropy

```
Probability Distribution
          │
          ▼
Predictability
          │
          ▼
Uncertainty
          │
          ▼
Entropy
          │
          ▼
Cryptographic Security
```

***

### 🌍 Real-World Examples

#### Passwords

Random passwords have higher entropy than common passwords.

***

#### Cryptographic Keys

Randomly generated keys maximize entropy and improve security.

***

#### Lottery

Winning the lottery is highly unlikely, so learning that you have won provides a large amount of information.

***

### 🔐 Cryptography Perspective

Entropy is widely used to evaluate:

* Password strength.
* Secret keys.
* Random number generators.
* Information leakage.
* Secure communication protocols.

Higher entropy generally means greater resistance against guessing and brute-force attacks.

***

### ⚠️ Common Mistakes

* Assuming entropy measures security directly.
* Confusing randomness with entropy.
* Believing entropy can be negative.
* Assuming equal outcomes always exist.
* Ignoring the underlying probability distribution.

***

### 📌 Key Takeaways

* Entropy measures average uncertainty.
* Entropy is always non-negative.
* Maximum entropy occurs for uniform distributions.
* Minimum entropy occurs for certain events.
* Entropy depends only on probability distribution.

***

### 🧠 Quick Revision

| Property     | Description              |
| ------------ | ------------------------ |
| Non-negative | $H(X)\ge0$               |
| Maximum      | Uniform distribution     |
| Minimum      | Certain event            |
| Depends On   | Probability distribution |
| Unit         | Bits                     |

***

### ❓ Practice Questions

#### Conceptual Questions

1. State the properties of Shannon Entropy.
2. When is entropy maximum?
3. When is entropy minimum?
4. Why does entropy depend only on probability?
5. Explain the Binary Entropy Function.

#### Analytical Questions

1. Compare uniform and non-uniform distributions.
2. Explain why entropy is zero for a certain event.
3. Discuss the importance of entropy properties in cryptography.

***

### 📝 Page Summary

The properties of Shannon Entropy explain how uncertainty behaves under different probability distributions. Entropy is always non-negative, reaches its maximum for uniformly distributed outcomes, and becomes zero when the outcome is certain. These properties provide the theoretical foundation for understanding randomness, secure key generation, password strength, and the security of cryptographic systems.
