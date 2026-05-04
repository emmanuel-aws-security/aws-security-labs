# VPC Lab — SG vs NACL Steps

----------------------------------
## 🔹 BASELINE — Confirm Working Access
----------------------------------

Setup:
- Public EC2
- Private EC2

Security Group:
- Private EC2 allows SSH (port 22) from public EC2

Test:
- SSH from public → private → works ✅

----------------------------------
## 🔹 Step 1: Create Custom NACL
----------------------------------

- Create new NACL
- Associate it with private subnet

----------------------------------
## 🔹 BREAK — Add DENY Rule
----------------------------------

Add rule in NACL:

- Type: SSH (22)
- Source: 0.0.0.0/0
- Action: DENY
- Rule number: (lower number = higher priority)

----------------------------------
## 🔹 Step 2: Test Again
----------------------------------

- SSH from public → private → fails ❌

----------------------------------
## 🔹 Step 3: Confirm Root Cause
----------------------------------

Check:
- Security Group still allows SSH ✅
- Instance running ✅
- Network ACL denies ❌

👉 Root cause = NACL blocking traffic

----------------------------------
## 🔹 FIX — Remove or Modify NACL Rule
----------------------------------

- Delete DENY rule
OR
- Change to ALLOW

----------------------------------
## 🔹 Step 4: Re-test
----------------------------------

- SSH from public → private → works ✅
