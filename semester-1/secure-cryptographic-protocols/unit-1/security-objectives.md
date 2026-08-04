# 🎯 Security Objectives

***

### 📖 Overview

Security objectives define the primary goals of protecting information and communication systems. They ensure that data remains secure from unauthorized access, modification, destruction, or disruption. These objectives serve as the foundation of modern cryptography and cybersecurity.

***

### 🎯 Why are Security Objectives Important?

* Protect sensitive information from unauthorized access.
* Ensure data remains accurate and unaltered.
* Keep systems and services available when needed.
* Build trust between users and organizations.
* Reduce security risks and cyber threats.

***

### 🔑 Core Security Objectives

#### 1. Confidentiality

* Ensures information is accessible only to authorized users.
* Prevents unauthorized disclosure of sensitive data.

**Example:** Encrypting online banking transactions using TLS.

***

#### 2. Integrity

* Ensures data is not modified or tampered with.
* Detects unauthorized changes to information.

**Example:** Verifying a downloaded file using a SHA-256 hash.

***

#### 3. Availability

* Ensures systems and data are available whenever authorized users need them.
* Protects against outages and denial-of-service attacks.

**Example:** Using backup servers and redundancy to keep websites online.

***

#### 4. Authentication

* Verifies the identity of users, devices, or systems.
* Prevents unauthorized access.

**Example:** Logging in with a username, password, and OTP.

***

#### 5. Authorization

* Determines what an authenticated user is allowed to access or perform.
* Implements access control policies.

**Example:** An administrator can modify user accounts, while a regular user cannot.

***

#### 6. Non-Repudiation

* Prevents a sender or receiver from denying an action or transaction.
* Achieved using digital signatures and audit logs.

**Example:** A digitally signed contract cannot later be denied by the signer.

***

### 🔄 Relationship Between Security Objectives

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
   Non-Repudiation (Records & Proof)
```

***

### 🌍 Real-World Example

Consider an online banking system:

* **Confidentiality:** Customer data is encrypted.
* **Integrity:** Transactions cannot be modified.
* **Availability:** Banking services are available 24/7.
* **Authentication:** Users log in using passwords and OTPs.
* **Authorization:** Customers can access only their own accounts.
* **Non-Repudiation:** Digital signatures provide proof of transactions.

***

### 📌 Key Takeaways

* Security objectives define the goals of information security.
* The six primary objectives are **Confidentiality, Integrity, Availability, Authentication, Authorization, and Non-Repudiation**.
* These objectives guide the design of secure cryptographic protocols and communication systems.
* Together, they help protect data, users, and digital infrastructure from cyber threats.

***

#### 💡 Note for this Course

The syllabus specifically mentions **"Security objectives as uncertainty reduction and leakage control."** In the **next topic**, you'll learn how cryptography achieves these objectives by **reducing an attacker's uncertainty** about secret information and **controlling information leakage**. This naturally connects **Security Objectives** with **Security as Uncertainty Reduction & Leakage Control**.
