# 📊 Random Variables & Probability

### 📖 Overview

Before information and uncertainty can be measured mathematically, we must understand two fundamental concepts: **Random Variables** and **Probability**.

A random event can have multiple possible outcomes, and each outcome occurs with a certain likelihood. Information Theory uses these probabilities to quantify uncertainty and ultimately derive Shannon Entropy.

Therefore, Random Variables and Probability serve as the mathematical foundation of Information Theory and modern cryptography.

***

### 🎯 Why Study Random Variables & Probability?

Random Variables and Probability are essential because they help us:

* Represent uncertain events mathematically.
* Assign probabilities to possible outcomes.
* Model real-world communication systems.
* Measure uncertainty.
* Build the foundation for Shannon Entropy.
* Analyze randomness in cryptographic systems.

Without these concepts, it is impossible to understand how entropy is calculated.

***

## 🎲 Random Variable

### 📖 Definition

A **Random Variable** is a variable whose value depends on the outcome of a random experiment.

Unlike ordinary variables, a random variable does not have a fixed value. Instead, its value is determined only after an experiment is performed.

Random variables are usually represented using capital letters such as:

```
X
Y
Z
```

The possible values taken by a random variable are represented using lowercase letters.

Example:

```
X = {A, B, C}
```

where:

* A, B, and C are possible outcomes.
* X is the random variable.

***

### 🌍 Examples

#### Example 1 – Coin Toss

Random Variable:

```
X = {Head, Tail}
```

Possible outcomes:

* Head
* Tail

***

#### Example 2 – Rolling a Dice

```
X = {1,2,3,4,5,6}
```

Possible outcomes:

* 1
* 2
* 3
* 4
* 5
* 6

***

#### Example 3 – Password Generator

Suppose a password generator selects one password from:

```
X = {Alpha, Bravo, Charlie, Delta}
```

Each selected password represents one outcome of the random variable.

***

## 📊 Types of Random Variables

Random Variables are generally classified into two categories.

### 1. Discrete Random Variable

A discrete random variable has a **countable number of possible outcomes**.

Examples:

* Coin toss
* Dice roll
* Lottery number
* Password selection

Most cryptographic applications use discrete random variables.

***

### 2. Continuous Random Variable

A continuous random variable can take **any value within a continuous range**.

Examples:

* Temperature
* Time
* Voltage
* Distance

Continuous random variables are more common in engineering and signal processing than in introductory cryptography.

***

## 📈 Probability

### 📖 Definition

**Probability** is the numerical measure of how likely an event is to occur.

It is represented by:

```
P(X)
```

The value of probability always satisfies:

```
0 ≤ P(X) ≤ 1
```

where:

* 0 means the event is impossible.
* 1 means the event is certain.

***

### Interpretation

| Probability     | Meaning          |
| --------------- | ---------------- |
| 0               | Impossible Event |
| Between 0 and 1 | Possible Event   |
| 1               | Certain Event    |

***

## 📋 Probability Distribution

A **Probability Distribution** specifies the probability associated with every possible outcome of a random variable.

Example:

| Outcome | Probability |
| ------- | ----------: |
| A       |        0.50 |
| B       |        0.30 |
| C       |        0.20 |

For every valid probability distribution:

```
P(A)+P(B)+P(C)=1
```

In general,

```
Σ P(xᵢ)=1
```

This means the probabilities of all possible outcomes must sum to **1**.

***

## ⚖️ Uniform Distribution

A **Uniform Distribution** occurs when all possible outcomes are equally likely.

Example:

Fair Coin

| Outcome | Probability |
| ------- | ----------: |
| Head    |         0.5 |
| Tail    |         0.5 |

Example:

Fair Dice

| Outcome | Probability |
| ------- | ----------: |
| 1       |         1/6 |
| 2       |         1/6 |
| 3       |         1/6 |
| 4       |         1/6 |
| 5       |         1/6 |
| 6       |         1/6 |

Uniform distributions generally produce greater uncertainty because no outcome is favored.

***

## 📉 Non-Uniform Distribution

A **Non-Uniform Distribution** occurs when different outcomes have different probabilities.

Example:

| Outcome | Probability |
| ------- | ----------: |
| A       |        0.70 |
| B       |        0.20 |
| C       |        0.10 |

Here, outcome **A** is much more likely than the others.

As one outcome becomes increasingly likely, uncertainty decreases.

***

## ➕ Expected Information

Suppose some events occur more frequently than others.

Should every event contribute equally to the total amount of information?

The answer is **No**.

Events that occur frequently contribute less information than rare events.

Therefore, Information Theory combines:

* Possible outcomes
* Their probabilities

to compute the **average information** produced by a random source.

This concept is called **Expected Information**, which leads directly to **Shannon Entropy** in the next page.

***

## 🔄 Concept Flow

```
Random Experiment
        │
        ▼
Random Variable
        │
        ▼
Possible Outcomes
        │
        ▼
Assign Probabilities
        │
        ▼
Probability Distribution
        │
        ▼
Expected Information
        │
        ▼
Shannon Entropy
```

***

## 🌍 Real-World Examples

### Example 1 – Coin Toss

Random Variable:

```
X = {H,T}
```

Both outcomes are equally likely.

***

### Example 2 – Weather Forecast

Random Variable:

```
X = {Rain, No Rain}
```

Possible probabilities:

| Outcome | Probability |
| ------- | ----------: |
| Rain    |        0.30 |
| No Rain |        0.70 |

***

### Example 3 – Password Generation

Suppose a system randomly generates one password from one million possibilities.

Each possible password represents one outcome of a random variable.

The larger the number of equally likely passwords, the greater the uncertainty.

***

## 🔐 Cryptography Perspective

Random Variables and Probability are fundamental to cryptography.

They are used in:

* Cryptographic key generation
* Password generation
* Random number generators
* Secure authentication
* Information-theoretic security
* Shannon Entropy calculations

Modern cryptographic algorithms rely on high-quality randomness to ensure strong security.

***

## ⚠️ Common Mistakes

* Confusing a random variable with its outcomes.
* Assuming all probability distributions are uniform.
* Using probabilities that do not sum to **1**.
* Treating probability as certainty.
* Ignoring unlikely outcomes when calculating distributions.

***

## 📌 Key Takeaways

* A Random Variable represents the outcome of a random experiment.
* Probability measures the likelihood of an event.
* Probability values always lie between **0** and **1**.
* The probabilities of all outcomes must sum to **1**.
* Uniform distributions produce greater uncertainty than non-uniform distributions.
* Expected Information forms the bridge to Shannon Entropy.

***

## 🧠 Quick Revision

| Concept                  | Meaning                                  |
| ------------------------ | ---------------------------------------- |
| Random Variable          | Represents random outcomes               |
| Probability              | Likelihood of an event                   |
| Probability Distribution | Probabilities assigned to all outcomes   |
| Uniform Distribution     | Equal probabilities                      |
| Non-Uniform Distribution | Unequal probabilities                    |
| Expected Information     | Average information from a random source |

***

## ❓ Practice Questions

### Conceptual Questions

1. Define a Random Variable with an example.
2. Differentiate between discrete and continuous random variables.
3. What is probability?
4. What is a probability distribution?
5. Explain the difference between uniform and non-uniform distributions.

### Analytical Questions

1. Why must the probabilities of all outcomes sum to one?
2. Why do uniform distributions produce greater uncertainty?
3. Explain how Random Variables and Probability prepare us for Shannon Entropy.

***

## 📝 Page Summary

Random Variables and Probability provide the mathematical language for describing uncertain events. A random variable represents the possible outcomes of an experiment, while probability quantifies how likely each outcome is. A probability distribution combines these probabilities into a complete model of the random source. These concepts naturally lead to the idea of **Expected Information**, which forms the basis for the mathematical definition of **Shannon Entropy** presented in the next page.
