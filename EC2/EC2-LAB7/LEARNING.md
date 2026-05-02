# EC2 Debug Lab — Case 2 Learnings

## 🔴 Core Insight
A working server can still be unreachable due to network restrictions.

## 🧠 Layered Debugging Understanding

### 1. Security Group (AWS)
- Controls external access
- If blocked → internet cannot reach instance

### 2. Port Listening (Service)
- If no service is listening → nothing responds

### 3. UFW Firewall (OS)
- Can block traffic even if AWS allows it

## 🔍 Key Debug Pattern

If:
- Local works ✅
- External fails ❌

👉 Problem = network layer (SG or firewall)

If:
- Local fails ❌

👉 Problem = service or port

## ⚠️ Common Mistake
Checking only one layer and assuming it is the problem.

## 🧾 Final Conclusion
Access requires alignment across:
- application
- port
- network
- firewall

Failure in any layer breaks the system.
