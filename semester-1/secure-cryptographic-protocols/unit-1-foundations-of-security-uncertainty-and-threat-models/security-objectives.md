# 🎯 Security Objectives

### 📖 Overview

Security objectives define the primary goals of protecting information, communication systems, and digital assets from unauthorized access, modification, disclosure, destruction, or disruption. They establish the fundamental requirements that every secure system must satisfy and serve as the cornerstone of modern cryptography, cybersecurity, and information security.

Every cryptographic protocol, whether used for secure messaging, online banking, cloud computing, or military communication, is designed to achieve one or more of these objectives. Understanding these objectives is essential before studying entropy, secrecy, or cryptographic algorithms.

***

### 🎯 Why are Security Objectives Important?

Security objectives provide a framework for designing, implementing, and evaluating secure information systems. They help organizations protect valuable digital assets and maintain trust in modern communication systems.

They are important because they:

* Protect sensitive information from unauthorized access.
* Ensure data remains accurate and unaltered.
* Keep systems and services available whenever required.
* Build trust between users, organizations, and systems.
* Reduce cybersecurity risks and defend against cyber threats.
* Form the foundation for designing secure cryptographic protocols.

***

### 🎓 Learning Objectives

After studying this chapter, you will be able to:

* Explain the objectives of information security.
* Describe the CIA Triad.
* Differentiate between authentication and authorization.
* Explain the importance of non-repudiation.
* Understand how cryptography helps achieve security objectives.
* Apply security objectives to real-world cybersecurity scenarios.

***

### 📚 Prerequisites

Before studying this topic, you should be familiar with:

* Basic computer systems
* Computer networks
* Information security fundamentals
* Digital communication concepts

***

## 🔑 Core Security Objectives

The fundamental security objectives are commonly represented by the **CIA Triad**, which forms the basis of modern information security.

```
           Information Security

                CIA Triad

         Confidentiality
               ▲
               │
Integrity ◄────────────► Availability
```

In addition to the CIA Triad, modern systems also require Authentication, Authorization, and Non-Repudiation.

***

### 1. Confidentiality

#### 📖 Definition

Confidentiality ensures that information is accessible **only to authorized users, systems, or processes**.

Unauthorized individuals should never be able to access or understand confidential information.

#### 🎯 Objective

Protect information from unauthorized disclosure.

#### 🔐 How Cryptography Helps

* Encryption
* Secure key management
* VPNs
* TLS/SSL
* Access control

#### 🌍 Example

Encrypting online banking transactions using **TLS** ensures that attackers cannot read sensitive financial information while it is transmitted over the Internet.

***

### 2. Integrity

#### 📖 Definition

Integrity ensures that information remains **accurate, complete, and unaltered** during storage or transmission.

Any unauthorized modification should be detectable.

#### 🎯 Objective

Protect information from unauthorized modification.

#### 🔐 How Cryptography Helps

* Cryptographic Hash Functions
* Message Authentication Codes (MACs)
* Digital Signatures

#### 🌍 Example

Verifying a downloaded software package using a **SHA-256 hash** confirms that the file has not been modified.

***

### 3. Availability

#### 📖 Definition

Availability ensures that authorized users can access systems, services, and information whenever required.

#### 🎯 Objective

Prevent service disruption.

#### Common Threats

* Denial-of-Service (DoS)
* Distributed Denial-of-Service (DDoS)
* Hardware failures
* Natural disasters
* Ransomware

#### Protection Methods

* Backup servers
* Redundancy
* Load balancing
* Disaster recovery
* Fault tolerance

#### 🌍 Example

Using redundant servers ensures that a banking website remains available even if one server fails.

***

### 4. Authentication

#### 📖 Definition

Authentication verifies the identity of users, devices, or systems before granting access.

#### 🎯 Objective

Prevent unauthorized users from accessing protected resources.

#### Common Methods

* Passwords
* One-Time Passwords (OTP)
* Biometrics
* Smart Cards
* Digital Certificates

#### 🌍 Example

Logging into an online banking application using a username, password, and OTP.

***

### 5. Authorization

#### 📖 Definition

Authorization determines **what an authenticated user is allowed to access or perform**.

Authentication answers:

> **Who are you?**

Authorization answers:

> **What are you allowed to do?**

#### 🌍 Example

A database administrator can modify records, while a regular employee can only view them.

***

### 6. Non-Repudiation

#### 📖 Definition

Non-repudiation ensures that neither the sender nor the receiver can later deny performing a particular action or transaction.

#### How It Is Achieved

* Digital Signatures
* Public Key Infrastructure (PKI)
* Audit Logs

#### 🌍 Example

A digitally signed contract provides legal proof that the signer approved the document.

***

## 🔄 Relationship Between Security Objectives

```
User
 │
 ▼
Authentication
 │
 ▼
Authorization
 │
 ▼
Access to Resources
 │
 ├── Confidentiality
 ├── Integrity
 └── Availability
 │
 ▼
Non-Repudiation
```

This diagram illustrates how authentication and authorization control access to protected resources, while confidentiality, integrity, and availability safeguard those resources. Non-repudiation provides evidence of actions performed within the system.

***

## 🌍 Real-World Example

Consider an online banking system.

| Security Objective | Practical Example                                                      |
| ------------------ | ---------------------------------------------------------------------- |
| Confidentiality    | Customer information is encrypted using TLS.                           |
| Integrity          | Transaction details are protected using digital signatures and hashes. |
| Availability       | Banking services remain available 24×7 through redundant servers.      |
| Authentication     | Customers log in using passwords and OTPs.                             |
| Authorization      | Customers can access only their own accounts.                          |
| Non-Repudiation    | Digital signatures provide proof of completed transactions.            |

***

## ⚠️ Common Mistakes

* Confusing **Authentication** with **Authorization**.
* Assuming encryption alone provides complete security.
* Ignoring Availability while focusing only on Confidentiality.
* Believing Integrity automatically guarantees Confidentiality.
* Assuming all security objectives are equally important in every application.

***

## 📌 Key Takeaways

* Security objectives define the goals of information security.
* The **CIA Triad** consists of Confidentiality, Integrity, and Availability.
* Authentication verifies identity.
* Authorization determines access permissions.
* Non-repudiation prevents denial of actions.
* Cryptography provides mechanisms to achieve these objectives.

***

## 🧠 Quick Revision

| Objective       | Purpose                           |
| --------------- | --------------------------------- |
| Confidentiality | Prevent unauthorized disclosure   |
| Integrity       | Prevent unauthorized modification |
| Availability    | Ensure continuous access          |
| Authentication  | Verify identity                   |
| Authorization   | Control permissions               |
| Non-Repudiation | Prevent denial of actions         |

***

## ❓ Practice Questions

### Conceptual Questions

1. Define security objectives.
2. Explain the CIA Triad with suitable examples.
3. Differentiate between authentication and authorization.
4. What is non-repudiation? Why is it important?
5. Explain how cryptography supports confidentiality.

### Analytical Questions

1. Can confidentiality exist without integrity? Justify your answer.
2. Explain the importance of availability in cloud computing.
3. Which security objective is most important in online banking? Explain your reasoning.

***

## 📝 Chapter Summary

Security objectives define the fundamental requirements that every secure information system must satisfy. The CIA Triad—Confidentiality, Integrity, and Availability—forms the foundation of information security, while Authentication, Authorization, and Non-Repudiation extend these principles to meet the requirements of modern digital systems. Together, these objectives guide the design, implementation, and evaluation of secure cryptographic protocols and communication systems.
