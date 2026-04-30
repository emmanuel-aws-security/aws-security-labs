# EC2 Lab 2 — Learnings

## 🔴 Core Risk
Opening SSH to 0.0.0.0/0 exposes the server to the entire internet.

## 💥 Real-World Impact
Attackers constantly scan for open SSH ports and attempt:
- brute-force login
- credential guessing
- automated attacks

## 🔍 How Attackers Find Servers
- Internet-wide scanning tools detect open ports
- Public IP ranges are continuously scanned
- Open port 22 is a common target

## ⚠️ Why This Is Dangerous
Even if login fails:
- repeated attempts can occur
- logs get flooded
- weak credentials can be exploited

## 🧠 Security Insight
Access should always be restricted to trusted IP addresses.

## 🔧 Correct Fix (next step)
- Restrict SSH access to specific IP:
  <your-ip>/32

## 🧾 Final Conclusion
Leaving SSH open to the internet significantly increases the attack surface of an EC2 instance.
