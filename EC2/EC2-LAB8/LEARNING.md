# EC2 Debug Lab — Case 3 Learnings

## 🧠 Core Concept
curl helps isolate where the failure exists by removing external variables.

## 🔍 Key Patterns

### ✔ Local works, external fails
- Problem = network layer
- Causes:
  - Security Group
  - Firewall (UFW)

### ❌ Local fails
- Problem = application/service
- Causes:
  - service stopped
  - port not listening

### ❌ Both fail
- Service is not running or broken

## 🧠 Why curl is powerful
- Tests server directly
- Removes DNS/browser issues
- Helps isolate layers quickly

## ⚠️ Common Mistake
Jumping straight to AWS settings without testing locally.

## 🧾 Final Conclusion
Always test locally first. It tells you whether the problem is inside the server or outside it.
