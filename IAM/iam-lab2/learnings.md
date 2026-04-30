# IAM Lab 1 — Learnings (Permission Testing)

## 🔴 Key Observation
Even though I had access to S3, I could only perform actions defined in the policy.

## 🧠 Core Concept Learned
IAM follows an explicit allow model:
- Only actions defined in the policy are allowed
- Everything else is automatically denied

## 🔍 Important Insight
IAM is not only about granting permissions — it is also about enforcing restrictions.

## ⚠️ Security Meaning
Read-only access protects data integrity by preventing:
- accidental deletion
- unauthorized uploads
- bucket modifications

## 🧾 Final Understanding
AWS IAM ensures strict control over actions by denying anything not explicitly permitted.
