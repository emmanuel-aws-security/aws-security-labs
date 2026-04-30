# EC2 Lab 1 — Learnings

## 🧠 Core Concept
Launching an EC2 instance is only the first step. Access and service verification are required to confirm functionality.

## 🔑 SSH Access
Access to EC2 is controlled using key pairs. Without the correct private key, login is not possible.

## 🌐 Connectivity Insight
There are two levels of access:
- Local (inside the server)
- External (from the internet)

Both must work for a service to be considered properly deployed.

## ⚠️ Common Mistake
Many users launch instances but fail to verify if services are actually running or accessible.

## 🧾 Final Conclusion
A working EC2 setup requires:
- Successful SSH access
- Running service
- Proper network configuration (security group)
