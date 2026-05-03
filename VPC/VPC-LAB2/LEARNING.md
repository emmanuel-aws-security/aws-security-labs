# VPC Lab — Route Table Learnings

## 🔴 Core Concept
0.0.0.0/0 represents all external traffic.

## 🧠 Key Insight
Internet access exists only when:
- traffic is routed to an Internet Gateway

## 🔍 What Happened
- Before:
  EC2 → route → IGW → internet

- After removal:
  EC2 → no route → request dropped

## ⚠️ Critical Understanding
Even if:
- EC2 is public
- Security Group allows traffic

👉 Without route → NO internet

## 🧠 Security Insight
Misconfigured route tables can:
- break applications
- isolate services unintentionally
- or expose systems if wrongly configured

## 🧾 Final Conclusion
Routing is the backbone of AWS networking.
No route = no communication.
