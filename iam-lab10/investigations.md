# Investigation — Root Cause Analysis

## 🧠 Problem
User has inconsistent access behavior across S3 actions.

Some actions work, others fail.

---

## 🔍 Step 1: IAM Policy Simulator

Tested actions:
- s3:ListBucket → Allowed
- s3:PutObject → Allowed
- s3:DeleteObject → Denied

Clicked simulation details:
- Allow source: user policy + group policy
- Deny source: explicit deny policy

---

## 🔍 Step 2: Trace All Permission Sources

### 1. User Policy
- Grants full S3 access

### 2. Group Policy
- Grants S3 read-only access

### 3. Explicit Deny Policy
- Blocks s3:DeleteObject

---

## ⚠️ Root Cause Identified
Even though multiple policies allow access, the explicit deny overrides all allow permissions.

---

## 🧠 Key Insight
AWS evaluates permissions from multiple sources:
- User policies
- Group policies
- Attached policies
- Explicit deny rules

Final decision depends on evaluation logic, not just “who has permission”.

---

## 🧾 Conclusion
The deny policy is the root cause of blocked actions, not missing permissions.
