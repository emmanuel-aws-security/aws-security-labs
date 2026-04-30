# IAM Lab 4 — Learnings

## 🧠 Core Concept
IAM roles are used to give permissions to AWS services instead of users.

## 🔑 Roles vs Access Keys

### Access Keys:
- Long-term credentials
- Must be stored somewhere
- Can be leaked or exposed

### IAM Roles:
- Temporary credentials
- Automatically provided by AWS
- No need to store secrets

## 🔍 What I Observed
The EC2 instance was able to access S3 without any access keys configured manually.

## ⚠️ Security Insight
Using access keys inside EC2 is risky because:
- Keys can be exposed in code or files
- Anyone with the key can access resources

IAM roles remove this risk by:
- Providing temporary credentials
- Managing access securely in the background

## 🧾 Final Conclusion
IAM roles are a safer and recommended way to grant permissions to AWS services compared to using access keys.
