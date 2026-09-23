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
During password cracking, a tool can test possible passwords and compare the resulting value against the available hash.

A simplified workflow is:

Password Candidates
        |
        v
   Cracking Tool
        |
        v
Generate/Test Candidate
        |
        v
Compare With Hash
        |
   +----+----+
   |         |
 Match     No Match
   |         |
   v         v
Success     Continue
4. Lab Environment

The practical exercise was performed in a controlled cybersecurity learning environment.

Operating System
Kali Linux
Password Cracking Tools
John the Ripper
Johnny
Networkwalks Password Cracking Tool
Target

An authorized password-protected PDF was used as the test target.

The purpose was to demonstrate password recovery techniques rather than attack a real user's account.

5. Methodology

The project was completed in the following stages.

Stage 1 – Prepare the Password-Cracking Environment

The Kali Linux environment was prepared for the password-cracking exercise.

The required password-cracking tools and supporting files were made available before starting the test.

Stage 2 – Password Cracking Using John the Ripper

John the Ripper was used to perform password recovery against the authorized password-protected PDF.

The general workflow was:

Protected PDF
     |
     v
Extract/Prepare Hash
     |
     v
John the Ripper
     |
     v
Password Candidates
     |
     v
Hash Comparison
     |
     v
Recovered Password

The cracking process tested password candidates against the extracted PDF hash.

Stage 3 – John the Ripper / Johnny

The Johnny graphical interface was also used to demonstrate the password-cracking process.

The interface displayed:

The target entry
Password field
Hash information
Supported format
Cracking status
Cracked-password result

The target was identified as a PDF format.

The cracking process successfully recovered the password.

Result
Status: CRACKED
Format: PDF
Recovered password: password1

The Johnny interface showed the recovered password after the cracking process completed successfully.

6. Networkwalks Password Cracking Tool

The second part of the exercise involved the Networkwalks password-cracking tool.

The tool systematically attempted password candidates against the authorized target.

Example process:

Trying: service       X
Trying: canada       X
Trying: hockey       X
Trying: killer       X
Trying: george       X
Trying: asdfgh       X
Trying: zxcvbn       X
Trying: qwertyuiop   X
Trying: 111222       X

MATCH password1      ✓

The tool eventually identified the correct password:

password1

The result was displayed as:

PASSWORD CRACKED SUCCESSFULLY

This demonstrated how weak and predictable passwords can potentially be recovered through password-guessing techniques.

7. Evidence

Screenshots were captured throughout the exercise to provide evidence of the practical work.

Evidence 1 – Networkwalks Password Cracking Result

The screenshot demonstrates the password candidates being tested and the successful match.

Key observation:

[+] MATCH password1 ✓

The tool subsequently displayed:

PASSWORD CRACKED SUCCESSFULLY
Screenshot

Place the corresponding screenshot in:

screenshots/networkwalks-password-cracking.png
Evidence 2 – Johnny / John the Ripper Result

The Johnny interface displayed the recovered password and confirmed that the PDF password had been successfully cracked.

Important information visible in the evidence includes:

Password
Hash
PDF format
Cracking status
Number of cracked entries
Screenshot

Place the corresponding screenshot in:

screenshots/johnny-password-cracked.png
8. Results

The password recovery exercise was successful using both approaches.

Method	Target	Result
Networkwalks Password Cracking Tool	Authorized PDF	Password recovered
John the Ripper / Johnny	Authorized PDF	Password recovered
Password identified	Lab credential	password1

The exercise demonstrated that password strength has a significant effect on resistance to password-guessing attacks.

9. Security Lessons Learned

This project provided several important cybersecurity lessons.

9.1 Weak Passwords Are Vulnerable

Short, predictable, or commonly used passwords can be significantly easier to recover.

9.2 Password Length Matters

Longer passwords/passphrases generally provide a larger search space and can increase resistance to guessing attacks.

9.3 Password Complexity Matters

Passwords should avoid:

Common words
Simple number sequences
Keyboard patterns
Personal information
Reused passwords
9.4 Password Reuse Is Dangerous

Using the same password across multiple services increases the potential impact of a compromised credential.

9.5 Strong Hashing Is Important

Modern systems should use password-specific password hashing mechanisms designed to make large-scale guessing expensive, together with appropriate salts.

9.6 Multi-Factor Authentication

MFA provides an additional layer of protection even when a password is compromised.

10. Defensive Recommendations

Organizations and individuals should consider:

Using long, unique passwords.
Using password managers.
Enabling multi-factor authentication.
Avoiding password reuse.
Using secure password hashing algorithms.
Applying appropriate password policies.
Monitoring authentication attempts.
Implementing account lockout/rate limiting where appropriate.
Protecting password hashes from unauthorized access.
Regularly reviewing credential security.
11. Skills Demonstrated

This project helped develop practical skills in:

Password security
Password cracking concepts
Hash analysis
John the Ripper
Johnny
Wordlists
Linux cybersecurity tools
Security testing methodology
Evidence collection
Technical documentation
Cybersecurity ethics
12. Project Structure

The recommended repository structure is:

networkwalks-B083-week3-password-cracking/
│
├── README.md
│
├── screenshots/
│   ├── networkwalks-password-cracking.png
│   └── johnny-password-cracked.png
│
├── documentation/
│   └── Week3-Technical-Documentation.md
│
└── notes/
    └── learning-notes.md
13. Ethical Considerations

Password-cracking tools are dual-use cybersecurity technologies.

They can be used for legitimate activities such as:

Security assessments
Digital forensics
Password auditing
Cybersecurity education
Authorized penetration testing

They should only be used against systems, accounts, files, or credentials for which the tester has explicit authorization.

This project was conducted strictly within an authorized cybersecurity training environment.

14. Conclusion

The Networkwalks B083 Week 3 project provided practical experience with password security and password recovery techniques.

Using both John the Ripper/Johnny and the Networkwalks password-cracking tool, I successfully demonstrated the recovery of a password from an authorized protected PDF.

The exercise reinforced an important cybersecurity principle:

Weak credentials can become a security vulnerability when exposed to systematic password-guessing techniques.

The practical experience gained from this project contributes to my understanding of offensive security techniques and, more importantly, how these techniques can be used to identify and strengthen weaknesses in defensive security controls.

Author

Adongo Peter Oduor
Cybersecurity Learner – Networkwalks B083

Focus: Cybersecurity | SOC | Defensive Security | Ethical Hacking

Acknowledgement

Special appreciation to Networkwalks and Waqas Karim, CCIE, for providing practical cybersecurity learning opportunities and hands-on laboratory exercises.

#Networkwalks #Cybersecurity #EthicalHacking #JohnTheRipper #PasswordSecurity #KaliLinux
