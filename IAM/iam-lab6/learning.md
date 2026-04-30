# IAM Lab 6 — Learnings

## 🧠 Core Concept
AWS IAM evaluates permissions using a strict hierarchy.

## 🔴 Key Rule
Explicit deny always overrides allow.

## 💥 What I Observed
Even though the user had an allow policy for S3:
- Access was still denied after adding a deny policy

## ⚠️ Why This Matters
This prevents accidental exposure of resources even when broader permissions exist elsewhere.

## 🧠 Security Insight
Deny rules act as a safety lock in IAM policy evaluation.

## 🧾 Final Conclusion
In AWS IAM, no allow permission can override an explicit deny.
