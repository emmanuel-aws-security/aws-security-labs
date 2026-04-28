# Investigation — Why Was Data Exposed?

## 🧠 Problem
S3 object is accessible publicly without authentication.

---

## 🔍 Step 1: Policy Simulator

Tested:
- Action: s3:GetObject

Result:
- ❌ (from IAM user perspective)

👉 But file was still accessible publicly

---

## 🔍 Step 2: Check Resource Policy (S3 Bucket)

- Found bucket policy allowing:
  - Principal: "*"
  - Action: s3:GetObject

---

## 🔥 Root Cause
Access was granted by bucket policy, not IAM user policy.

---

## ⚠️ Key Insight
IAM policies are not the only control layer.

S3 bucket policies can:
- grant access externally
- bypass IAM user restrictions

---

## 🧾 Conclusion
Public exposure was caused by bucket-level permission, not IAM misconfiguration.
