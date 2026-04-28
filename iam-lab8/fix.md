# IAM Mini Attack Scenario — Fix

## 🔧 Step 1: Remove Dangerous Policy
- Detached AdministratorAccess from user

---

## 🔐 Step 2: Apply Least Privilege Policy

Apply custom policy S3 Read only



🔧 Step 3: Attach Policy
Attached restricted policy to user


🧪 Step 4: Re-Test Access
S3 read allowed
EC2 creation denied
S3 upload denied
