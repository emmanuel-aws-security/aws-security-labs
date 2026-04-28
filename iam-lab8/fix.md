# IAM Mini Attack Scenario — Fix

## 🔧 Step 1: Remove Dangerous Policy
- Detached AdministratorAccess from user

---

## 🔐 Step 2: Apply Least Privilege Policy

Created custom policy:

```json id="atk6"
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket",
        "s3:GetObject"
      ],
      "Resource": "*"
    }
  ]
}


🔧 Step 3: Attach Policy
Attached restricted policy to user


🧪 Step 4: Re-Test Access
S3 read allowed
EC2 creation denied
S3 upload denied
