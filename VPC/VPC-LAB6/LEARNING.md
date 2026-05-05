# VPC Lab — Flow Logs Learnings

## 🔴 Core Concept
Flow Logs show network-level traffic metadata.

## 🧠 Key Insight
You don’t see packets—you see:
- source IP
- destination IP
- action (ACCEPT / REJECT)

## 🔍 What Happened
- Allowed traffic → ACCEPT logged
- Blocked traffic → REJECT logged

## ⚠️ Critical Understanding
Flow Logs do NOT stop traffic—they only record it.

## 🧠 Real-World Use Case
Used for:
- security monitoring
- incident investigation
- detecting misconfigurations

## 🧾 Final Conclusion
Flow Logs = visibility layer for VPC traffic.
