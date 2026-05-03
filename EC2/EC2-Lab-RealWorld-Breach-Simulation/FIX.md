# EC2 Breach Simulation — Fix & Remediation

## 🔧 Fix 1 — Restrict SSH Access
- Change Security Group:
  FROM: 0.0.0.0/0
  TO: your IP /32

## 🔧 Fix 2 — Remove Hardcoded Credentials
rm creds.txt

## 🔧 Fix 3 — Use IAM Role Instead
- Attach IAM role to EC2
- Remove dependency on static keys

## 🔧 Fix 4 — Harden Security Group
- Allow only required ports:
  - SSH (restricted)
  - HTTP if needed

## 🔧 Fix 5 — Validate Fix
- Try SSH from another IP → denied
- Confirm no sensitive files exist
- Confirm IAM role works via AWS CLI

## 🧠 Final State
- No exposed credentials
- Restricted access
- Secure IAM-based permissions
