# Attack Simulation

## 🎯 Goal
Simulate how weak cloud security configurations can expose infrastructure to attackers.

---

## 🔥 Weak Configurations Introduced

### 1. Public EC2 Exposure
- EC2 deployed in public subnet
- public IP assigned

### 2. SSH Open to Internet
Security Group:
- Port 22 open to:
0.0.0.0/0

Risk:
- brute-force attempts
- unauthorized access attempts

---

### 3. Public S3 Exposure
- Bucket/object made public

Risk:
- unauthorized data access
- accidental data leak

---

### 4. Excessive Permissions
IAM user configured with broad permissions.

Risk:
- privilege abuse
- expanded attacker access

---

## 🧠 Simulated Attacker Thinking

If attacker gains EC2 access:
- inspect files
- search for credentials
- access AWS resources
- move across environment

---

## ⚠️ Security Insight
Cloud attacks usually begin with:
- exposed services
- weak permissions
- visibility failures
