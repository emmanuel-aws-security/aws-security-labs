# VPC Lab — SG vs NACL Learnings

## 🔴 Core Difference

### Security Groups
- Applied to instances
- Stateful (auto allows return traffic)
- Only ALLOW rules

### NACL
- Applied to subnet
- Stateless (must allow both directions)
- Supports ALLOW and DENY

## 🧠 Key Insight
Even if Security Group allows traffic:

👉 NACL can still block it

## 🔍 What Happened
- SG allowed SSH
- NACL denied SSH
- Result = connection failed

## ⚠️ Critical Rule
Explicit DENY (NACL) overrides ALLOW (SG)

## 🧠 Real-World Impact
Misconfigured NACLs can:
- break applications
- block internal communication
- cause hard-to-debug issues

## 🧾 Final Conclusion
AWS networking is layered:
- Instance level (SG)
- Subnet level (NACL)

Both must allow traffic.
