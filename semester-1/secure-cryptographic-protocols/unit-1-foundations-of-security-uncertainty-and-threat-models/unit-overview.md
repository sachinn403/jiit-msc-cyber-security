# 📖 Unit Overview

## 📖 Unit Overview

> **Unit 1 – Foundations of Security, Uncertainty and Threat Models**

***

### Introduction

Cryptography is the science of protecting information and communication against unauthorized access, modification, disclosure, and destruction. It combines mathematics, computer science, and engineering to provide mechanisms that ensure secure communication over insecure channels.

In today's digital world, cryptography forms the backbone of secure systems used in online banking, e-commerce, cloud computing, secure messaging, digital signatures, blockchain technology, and national defense. Every time a user logs into a website using HTTPS, transfers money online, or sends an encrypted message, cryptographic protocols operate behind the scenes to ensure confidentiality, integrity, authentication, and trust.

However, understanding cryptography begins **before studying encryption algorithms**. A fundamental question arises:

> **What does it actually mean for a system to be secure?**

This question cannot be answered simply by studying algorithms like AES or RSA. Instead, we must first understand the theoretical foundations of security itself.

This unit introduces the mathematical and conceptual principles that form the basis of modern cryptography. It explores how security can be measured, how uncertainty can be quantified using information theory, how information leakage occurs, what assumptions are made about attackers, and under what conditions perfect secrecy can be achieved.

Rather than focusing immediately on cryptographic algorithms, Unit 1 develops the **information-theoretic perspective of security**, which serves as the foundation for the remainder of the course.

***

### Why This Unit Matters

Every secure communication system depends on several fundamental questions:

* What information must remain secret?
* How can secrecy be measured mathematically?
* How much information does an attacker gain during an attack?
* How can uncertainty about secret information be quantified?
* What assumptions are made about an attacker's capabilities?
* When can a cryptographic system be considered perfectly secure?

Without answering these questions, it is impossible to correctly understand or evaluate any cryptographic protocol.

This unit establishes the theoretical framework required to answer these questions and prepares students for the cryptographic algorithms and protocols covered in later units.

***

### Learning Objectives

After completing this unit, you will be able to:

* Explain the objectives of information security.
* Describe security as uncertainty reduction and leakage control.
* Understand the role of information theory in cryptography.
* Compute Shannon entropy for various probability distributions.
* Interpret conditional entropy and mutual information.
* Explain the concept of perfect secrecy.
* Demonstrate why the One-Time Pad achieves perfect secrecy.
* Differentiate between computational and information-theoretic security.
* Identify different attacker models and their capabilities.
* Analyze brute-force attacks and password entropy.
* Distinguish between encryption, hashing, and encoding.

***

### Prerequisites

Before studying this unit, students should be familiar with:

* Basic computer systems
* Computer networking fundamentals
* Information security fundamentals
* Elementary probability
* Binary number system
* Basic mathematical notation
* Programming fundamentals (Python is recommended for laboratory exercises)

No prior knowledge of advanced cryptography is assumed.

***

### Where This Unit Fits in Cryptography

Cryptography is built upon multiple layers of knowledge.

```
Mathematics
      │
      ▼
Information Theory
      │
      ▼
Security Models
      │
      ▼
Cryptographic Algorithms
      │
      ▼
Cryptographic Protocols
      │
      ▼
Secure Systems
```

Unit 1 focuses primarily on the **first three layers**:

* Mathematical foundations
* Information theory
* Security models

These concepts provide the theoretical basis for all subsequent topics in modern cryptography.

***

### Unit Roadmap

The topics in this unit are arranged in a logical progression.

```
Security Objectives
        │
        ▼
Security as Uncertainty Reduction
        │
        ▼
Shannon Entropy
        │
        ▼
Conditional Entropy
        │
        ▼
Mutual Information
        │
        ▼
Perfect Secrecy
        │
        ▼
One-Time Pad
        │
        ▼
Computational vs Information-Theoretic Security
        │
        ▼
Attacker Models
        │
        ▼
Brute-Force Attacks
        │
        ▼
Password Entropy
        │
        ▼
Basic Threat Landscape
        │
        ▼
Encryption vs Hashing vs Encoding
```

Each topic builds upon the previous one, creating a complete understanding of security from an information-theoretic perspective.

***

### Connection with Future Units

The concepts introduced in Unit 1 serve as prerequisites for all remaining units of the course.

* **Unit 2** introduces symmetric-key cryptography and cryptographic primitives.
* **Unit 3** focuses on public-key cryptography, key exchange, and digital signatures.
* **Unit 4** explores secure cryptographic protocols and their real-world applications.

A solid understanding of entropy, secrecy, uncertainty, and attacker models is essential before studying these advanced topics.

***

### Real-World Motivation

The concepts studied in this unit have direct applications in modern cybersecurity.

| Concept             | Real-World Application                    |
| ------------------- | ----------------------------------------- |
| Security Objectives | Secure system architecture                |
| Shannon Entropy     | Password strength evaluation              |
| Conditional Entropy | Information leakage analysis              |
| Mutual Information  | Side-channel attack analysis              |
| Perfect Secrecy     | Military-grade secure communications      |
| One-Time Pad        | Intelligence and diplomatic communication |
| Attacker Models     | Threat modeling and penetration testing   |
| Password Entropy    | Authentication system design              |
| Brute-Force Attacks | Password auditing and security testing    |

These examples demonstrate that the theoretical concepts introduced in this unit are directly applicable to the design and analysis of modern secure systems.

***

### Expected Learning Outcomes

Upon successful completion of this unit, students will be able to:

* Apply information-theoretic concepts to analyze security problems.
* Quantify uncertainty using entropy-based measures.
* Evaluate information leakage in communication systems.
* Explain the principles of perfect secrecy.
* Analyze the capabilities of different attacker models.
* Assess the security of passwords using entropy.
* Build a strong conceptual foundation for advanced cryptographic protocols.

***

### Unit Summary

Unit 1 establishes the theoretical and mathematical foundations of modern cryptography. It introduces the objectives of information security, the concept of uncertainty and information leakage, entropy-based measures, perfect secrecy, attacker models, brute-force attacks, password entropy, and the distinction between encryption, hashing, and encoding.

These concepts form the intellectual foundation of cryptography and prepare students for the algorithmic and protocol-oriented topics explored in later units.

***

### Key Takeaways

* Cryptography is founded on mathematics, information theory, and security principles.
* Security can be analyzed in terms of uncertainty and information leakage.
* Entropy provides a mathematical measure of uncertainty.
* Perfect secrecy represents the strongest form of security.
* Attacker models determine the assumptions under which cryptographic systems are evaluated.
* Unit 1 provides the conceptual foundation required for all subsequent units of this course.
