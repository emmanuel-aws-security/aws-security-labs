# S3 Lab — IAM vs Bucket Policy Learnings

## 🔴 Core Concept
There are two layers of access control:

### 1. IAM Policy
- Controls what a user/role is allowed to do

### 2. Bucket Policy
- Controls what the resource allows

## 🧠 Key Insight
Both must allow access for the request to succeed.

## 🔍 What Happened
- IAM allowed access
- Bucket policy denied access
- Result → request failed

## ⚠️ Critical Rule
Explicit DENY in bucket policy always overrides IAM allow.

## 🧠 Real-World Meaning
Most access issues in AWS come from conflicts between IAM and resource policies.

## 🧾 Final Conclusion
IAM is identity-level control. Bucket policy is resource-level control. Both must align.
