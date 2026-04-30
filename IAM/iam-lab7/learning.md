# IAM Lab 7 — Learnings

## 🔐 Why MFA is Important
Multi-Factor Authentication adds an extra layer of security beyond passwords.

Even if a password is stolen:
- Access is still blocked without the MFA code

## 🔴 Why Password Alone is Weak
Passwords can be:
- guessed
- reused from other sites
- leaked in data breaches
- brute-forced

## 🧠 Security Insight
The root account is the most powerful identity in AWS. If compromised, it gives full control over the entire AWS environment.

## ⚠️ Best Practice
- Always enable MFA on root account
- Avoid using root for daily operations

## 🧾 Final Conclusion
Strong passwords alone are not enough. MFA is required to protect critical cloud accounts.
