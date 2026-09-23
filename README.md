# Networkwalks B083 – Week 3
## Password Cracking and Password Security Assessment

![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-red)
![Platform](https://img.shields.io/badge/Platform-Kali%20Linux-blue)
![Tool](https://img.shields.io/badge/Tool-John%20the%20Ripper-black)
![Batch](https://img.shields.io/badge/Networkwalks-B083-green)

## Project Overview

This project was completed as part of the **Networkwalks B083 Cybersecurity Training – Week 3**.

The project focused on understanding password security and demonstrating how password-cracking techniques can be used in an authorized cybersecurity laboratory environment.

Two approaches were explored:

1. Password cracking using **John the Ripper (JTR/Johnny)**.
2. Password cracking using the **Networkwalks password-cracking tool**.

The exercise demonstrated how weak or predictable passwords can be recovered through systematic password-guessing techniques and highlighted the importance of strong password security.

> **Ethical Notice:**  
> All password-cracking activities documented in this project were performed in an authorized learning/laboratory environment for cybersecurity education. No unauthorized accounts, systems, or credentials were targeted.

---

# 1. Objectives

The main objectives of this project were to:

- Understand the concept of password cracking.
- Understand the difference between passwords and password hashes.
- Learn how password-cracking tools operate.
- Gain practical experience with John the Ripper.
- Use the Johnny graphical interface for John the Ripper.
- Perform password recovery against an authorized protected PDF.
- Use the Networkwalks password-cracking tool.
- Compare the practical workflow of different password-cracking tools.
- Document the process using screenshots.
- Understand the security risks associated with weak passwords.
- Learn defensive techniques for protecting credentials.

---

# 2. Tools and Technologies

The following tools were used during the project:

| Tool | Purpose |
|---|---|
| Kali Linux | Cybersecurity testing environment |
| John the Ripper (JTR) | Password/hash cracking |
| Johnny | Graphical interface for John the Ripper |
| Networkwalks Password Cracking Tool | Password recovery exercise |
| Wordlist | Password candidate source |
| Protected PDF | Authorized target used for the exercise |
| Screenshots | Evidence and documentation |

---

# 3. Password Cracking Concepts

Password cracking is the process of attempting to recover a password from a password hash or protected authentication mechanism.

A password is normally not stored directly by a secure system. Instead, a system may store a representation such as a hash.

For example:

```text
Password
   |
   v
Hashing Algorithm
   |
   v
Password Hash
