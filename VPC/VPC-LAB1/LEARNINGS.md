# VPC Lab 1 — Learnings

## 🔴 Core Concept
Subnets are not “public” or “private” by default—routing determines their behavior.

## 🧠 Key Insight
A subnet becomes public only when:
- It has a route to an Internet Gateway

## 🔍 What Happened
- Public subnet:
  - Route → IGW → internet access

- Private subnet:
  - No IGW route → no internet access

## ⚠️ Common Mistake
Assuming subnet type is automatic instead of controlled by routing.

## 🧠 Security Insight
Private subnets provide isolation by removing direct internet exposure.

## 🧾 Final Conclusion
Network design in AWS is controlled by:
- Route tables
- Gateways
Not labels like “public” or “private”
