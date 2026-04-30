# EC2 Lab 3 — Learnings

## 🔴 Core Risk
Opening unnecessary ports increases the attack surface of the server.

## 💥 Real-World Impact
Attackers scan for open ports to find vulnerable services such as:
- FTP (21)
- Database ports (3306)
- Application ports (8080)

## ⚠️ Why This Is Dangerous
Even if no service is running:
- attackers still detect open ports
- misconfigurations can expose future services

## 🧠 Security Insight
Security groups should follow least privilege:
- only allow required ports
- restrict access where possible

## 🔧 Correct Practice
- SSH restricted to trusted IP
- HTTP only if needed
- all other ports closed

## 🧾 Final Conclusion
A properly configured security group minimizes exposure and reduces attack opportunities.
