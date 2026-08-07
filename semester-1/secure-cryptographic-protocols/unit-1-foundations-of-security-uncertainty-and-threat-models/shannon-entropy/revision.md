# 📝 Revision

### 📖 Overview

This page provides a concise revision of the Shannon Entropy chapter. It summarizes the key concepts, formulas, properties, applications, and important examination points to facilitate quick review before examinations or classroom discussions.

***

### 📐 Formula Sheet

#### 1. Self Information

$$
I(x)=-\log_{2}\!\big(P(x)\big)
$$

***

#### 2. Shannon Entropy

$$
H(X)=-
\sum_{i=1}^{n}
P(x_i)\log_{2}\!\big(P(x_i)\big)
$$

***

#### 3. Maximum Entropy

For **n equally likely outcomes**,

$$
H_{\max}=\log_{2}(n)
$$

***

#### 4. Binary Entropy Function

$$
H(p)=
-p\log_{2}(p)
-(1-p)\log_{2}(1-p)
$$

***

#### 5. Password Entropy

$$
H=L\times\log_{2}(N)
$$

where

* $L$ = Password Length
* $N$ = Character Set Size

***

### 📚 Important Definitions

#### Shannon Entropy

The **average amount of information** produced by a random source.

***

#### Self Information

The amount of information associated with a **single event**.

***

#### Information Content

The amount of information gained after observing an event.

***

#### Random Variable

A variable whose value depends on the outcome of a random experiment.

***

#### Probability Distribution

A mathematical description of the probabilities associated with every possible outcome of a random variable.

***

### 📌 Important Properties

* Entropy is always non-negative.
* Entropy is measured in **bits** when using $\log\_2$.
* Entropy is maximum when all outcomes are equally likely.
* Entropy is minimum when an event is certain.
* Entropy depends only on the probability distribution.
* Higher entropy indicates greater uncertainty.
* Lower entropy indicates greater predictability.

***

### 🔄 Concept Flow

```
Information Theory
        │
        ▼
Random Variable
        │
        ▼
Probability
        │
        ▼
Probability Distribution
        │
        ▼
Information Content
        │
        ▼
Self Information
        │
        ▼
Expected Information
        │
        ▼
Shannon Entropy
        │
        ▼
Cryptographic Applications
```

***

### 🔐 Applications

Shannon Entropy is widely used in:

* Password Strength Analysis
* Cryptographic Key Generation
* Random Number Generators
* Secure Communication
* Information Leakage Analysis
* Malware Detection
* Data Compression
* Digital Forensics

***

### ⚠️ Common Mistakes

* Forgetting the negative sign in the entropy formula.
* Using logarithms with the wrong base.
* Using probabilities that do not sum to **1**.
* Confusing **Self Information** with **Shannon Entropy**.
* Assuming higher entropy always guarantees security.
* Rounding intermediate values too early.

***

### 🧠 Quick Revision

#### Remember

* High Probability → Low Information
* Low Probability → High Information
* Equal Probabilities → Maximum Entropy
* Certain Event → Zero Entropy
* Entropy measures **Average Uncertainty**

***

#### Formula Map

```
Probability
      │
      ▼
Information Content
      │
      ▼
Self Information
      │
      ▼
Expected Value
      │
      ▼
Shannon Entropy
```

***

### 📊 Comparison Table

| Concept             | Meaning                                           |
| ------------------- | ------------------------------------------------- |
| Information Theory  | Mathematical study of information and uncertainty |
| Random Variable     | Represents uncertain outcomes                     |
| Probability         | Likelihood of an event                            |
| Information Content | Information contained in a single event           |
| Self Information    | Information of one event                          |
| Shannon Entropy     | Average uncertainty                               |
| High Entropy        | High unpredictability                             |
| Low Entropy         | High predictability                               |

***

### ❓ Practice Questions

#### Very Short Questions

1. Define Shannon Entropy.
2. What is Self Information?
3. State the Shannon Entropy formula.
4. What is the unit of entropy?
5. Who introduced Shannon Entropy?

***

#### Short Answer Questions

1. Explain Information Content.
2. Define Self Information with formula.
3. Explain Shannon Entropy.
4. Discuss the properties of Shannon Entropy.
5. Explain why entropy is maximum for uniform distributions.

***

#### Long Answer Questions

1. Derive the Shannon Entropy formula.
2. Explain the applications of Shannon Entropy in cybersecurity.
3. Discuss the properties and interpretation of Shannon Entropy.
4. Explain the relationship between probability, information, and entropy.
5. Discuss the importance of Shannon Entropy in modern cryptography.

***

#### Numerical Problems

1. Calculate the entropy of a fair coin.
2. Calculate the entropy for

| Outcome | Probability |
| ------- | ----------: |
| A       |         0.5 |
| B       |         0.3 |
| C       |         0.2 |

3. Calculate the entropy of a fair die.
4. Compare the entropy of a fair coin and a biased coin.
5. Compute the entropy for four equally likely outcomes.

***

### 🎯 Examination Tips

* Always write the entropy formula before substitution.
* Mention the logarithm base.
* Show every calculation step.
* Write the final answer in **bits**.
* Interpret the entropy value after every numerical problem.
* Practice both theoretical and numerical questions.

***

### 📝 Chapter Summary

Shannon Entropy, introduced by Claude Shannon in 1948, provides a mathematical measure of the average uncertainty or information produced by a random source. It is derived from the concept of Self Information and depends entirely on the probability distribution of the outcomes. Entropy is fundamental to Information Theory and serves as the theoretical foundation for modern cryptography, secure communication, password analysis, random number generation, data compression, and information leakage analysis. Understanding Shannon Entropy is essential before studying advanced concepts such as Conditional Entropy, Mutual Information, and Perfect Secrecy.

***

### ➡️ Next Topic

The next topic in this unit is **📊 Conditional Entropy**, where we study how the uncertainty of one random variable changes when information about another random variable is already known.

This concept extends Shannon Entropy and forms the basis for understanding **Mutual Information**, **Information Leakage**, and **Perfect Secrecy**.
