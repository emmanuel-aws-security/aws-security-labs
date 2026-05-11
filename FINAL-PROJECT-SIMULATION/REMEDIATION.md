# Remediation Process

## 🎯 Goal
Reduce attack surface and secure the environment.

---

## 🔧 Fixes Applied

### SSH Hardening
Before:
0.0.0.0/0

After:
MY-IP/32

Result:
- reduced external exposure

---

### S3 Protection
Actions:
- removed public access
- blocked public bucket policies

Result:
- restricted unauthorized access

---

### IAM Hardening
Actions:
- removed unnecessary permissions
- used IAM roles instead of access keys

Result:
- reduced credential exposure risk

---

### Network Segmentation
Actions:
- separated public/private resources
- restricted internal communication

Result:
- reduced lateral movement opportunities

---

## 🧠 Key Lesson
Security is strongest when:
- multiple layers work together
NOT
- relying on one control alone.
