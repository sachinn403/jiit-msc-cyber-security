# 🧮 Solved Numerical Examples

### 📖 Overview

Understanding Shannon Entropy requires not only theoretical knowledge but also the ability to solve numerical problems. This page presents step-by-step solutions to commonly encountered entropy calculations.

Each example demonstrates how to apply the Shannon Entropy formula to different probability distributions and interpret the resulting entropy value.

***

### 📐 Shannon Entropy Formula

The Shannon Entropy of a random variable is given by

$$
H(X)=-
\sum_{i=1}^{n}
P(x_i)\log_{2}\!\big(P(x_i)\big)
$$

where:

* $H(X)$ = Shannon Entropy
* $P(x\_i)$ = Probability of the $i^{th}$ outcome
* $\log\_2$ = Logarithm to base 2

***

## 🧮 Example 1 – Fair Coin

### Given

A fair coin has two equally likely outcomes.

| Outcome | Probability |
| ------- | ----------: |
| Head    |         0.5 |
| Tail    |         0.5 |

***

### Formula

$$
H(X)=-
\sum P(x)\log_{2}(P(x))
$$

***

### Solution

$$
H(X)=-
[(0.5\times\log_{2}0.5)
+
(0.5\times\log_{2}0.5)]
$$

Since

$$
\log_{2}(0.5)=-1
$$

Therefore,

$$
H(X)=-
[(0.5\times-1)
+
(0.5\times-1)]
$$

$$
H(X)=-
(-0.5-0.5)
$$

$$
H(X)=1
$$

***

### Answer

$$
\boxed{H(X)=1\text{ bit}}
$$

***

### Interpretation

A fair coin has maximum uncertainty because both outcomes are equally likely.

***

## 🧮 Example 2 – Biased Coin

### Given

| Outcome | Probability |
| ------- | ----------: |
| Head    |         0.9 |
| Tail    |         0.1 |

***

### Formula

$$
H(X)=-
\sum P(x)\log_{2}(P(x))
$$

***

### Solution

$$
H(X)=-
[(0.9\times\log_{2}0.9)
+
(0.1\times\log_{2}0.1)]
$$

Using

$$
\log_{2}(0.9)\approx-0.152
$$

$$
\log_{2}(0.1)\approx-3.322
$$

Substituting,

$$
H(X)=-
[(0.9\times-0.152)
+
(0.1\times-3.322)]
$$

$$
H(X)=-
(-0.1368-0.3322)
$$

$$
H(X)\approx0.469\text{ bits}
$$

***

### Answer

$$
\boxed{H(X)\approx0.469\text{ bits}}
$$

***

### Interpretation

Because one outcome is highly likely, uncertainty is much lower than in a fair coin.

***

## 🧮 Example 3 – Three Equal Outcomes

### Given

| Outcome | Probability |
| ------- | ----------: |
| A       |         1/3 |
| B       |         1/3 |
| C       |         1/3 |

***

### Solution

$$
H(X)=-
3\left(
\frac13
\times
\log_{2}\frac13
\right)
$$

Since

$$
\log_{2}(3)\approx1.585
$$

Therefore,

$$
H(X)\approx1.585\text{ bits}
$$

***

### Answer

$$
\boxed{H(X)\approx1.585\text{ bits}}
$$

***

### Interpretation

Equal probability distributions maximize entropy.

***

## 🧮 Example 4 – Unequal Probability Distribution

### Given

| Outcome | Probability |
| ------- | ----------: |
| A       |         0.5 |
| B       |         0.3 |
| C       |         0.2 |

***

### Solution

$$
H(X)=-
[(0.5\log_20.5)
+
(0.3\log_20.3)
+
(0.2\log_20.2)]
$$

Using

$$
\log_20.5=-1
$$

$$
\log_20.3\approx-1.737
$$

$$
\log_20.2\approx-2.322
$$

Therefore,

$$
H(X)\approx1.485\text{ bits}
$$

***

### Answer

$$
\boxed{H(X)\approx1.485\text{ bits}}
$$

***

### Interpretation

Since the probabilities are unequal, the entropy is lower than the maximum possible entropy for three equally likely outcomes.

***

## 🧮 Example 5 – Fair Dice

### Given

A fair die has six equally likely outcomes.

$$
P(x)=\frac16
$$

***

### Formula

For equally likely outcomes,

$$
H(X)=\log_{2}n
$$

where

$$
n=6
$$

***

### Solution

$$
H(X)=\log_{2}6
$$

$$
H(X)\approx2.585
$$

***

### Answer

$$
\boxed{H(X)\approx2.585\text{ bits}}
$$

***

### Interpretation

A fair die has greater uncertainty than a fair coin because it has more equally likely outcomes.

***

### 📊 Comparison of Examples

| Example              |    Entropy |
| -------------------- | ---------: |
| Fair Coin            | 1.000 bits |
| Biased Coin          | 0.469 bits |
| Three Equal Outcomes | 1.585 bits |
| Unequal Distribution | 1.485 bits |
| Fair Die             | 2.585 bits |

***

### 📌 Key Observations

* Equal probability distributions produce higher entropy.
* Biased distributions reduce uncertainty.
* Increasing the number of equally likely outcomes increases entropy.
* Shannon Entropy measures the average uncertainty of a random source.

***

### ⚠️ Common Mistakes

* Forgetting the negative sign.
* Using logarithms with the wrong base.
* Using probabilities that do not sum to 1.
* Rounding intermediate values too early.

***

### 🧠 Quick Revision

* Fair Coin → **1 bit**
* Biased Coin → **0.469 bits**
* Three Equal Outcomes → **1.585 bits**
* Unequal Distribution → **1.485 bits**
* Fair Die → **2.585 bits**

***

### ❓ Practice Problems

1. Calculate the entropy of a fair four-sided die.
2. Calculate the entropy for probabilities (0.6, 0.4).
3. Calculate the entropy for probabilities (0.25, 0.25, 0.25, 0.25).
4. Compare the entropy of a fair coin and a biased coin.
5. Explain why entropy increases with the number of equally likely outcomes.

***

### 📝 Page Summary

This page demonstrated the calculation of Shannon Entropy for various probability distributions using step-by-step numerical examples. These examples illustrate how entropy changes with probability and provide a practical foundation for solving examination and classroom problems.
