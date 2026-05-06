# S3 Lab — Bucket Policy Learnings

## 🔴 Core Concept
Bucket policies are JSON-based rules that control access to S3 resources.

## 🧠 Key Insight
Access is defined by:
- Effect (Allow / Deny)
- Action (what can be done)
- Resource (what is affected)

## 🔍 What Happened
- No policy → private access
- Public read policy → open access
- Policy removed → access blocked again

## ⚠️ Security Risk
Using:
"Principal": "*"

means anyone on the internet can access your data.

## 🧠 Real-World Meaning
Many S3 data leaks happen due to overly permissive bucket policies.

## 🧾 Final Conclusion
Bucket policies must be carefully written to avoid exposing sensitive data.
