# VPC Lab — Subnet Isolation Learnings

## 🔴 Core Concept
Instances inside the same VPC are NOT automatically allowed to communicate.

## 🧠 Key Insight
Security Groups control:
- instance-to-instance communication

Without rules:
- no traffic flows internally

## 🔍 What Happened
- Both EC2 instances exist in same VPC
- No inbound rule allowed traffic
- Connection failed

## ⚠️ Critical Misconception
Same network ≠ automatic trust

## 🧠 Real-World Impact
This prevents:
- lateral movement in attacks
- automatic internal exposure
- uncontrolled service access

## 🧾 Final Conclusion
Every internal connection must be explicitly allowed at Security Group level.
