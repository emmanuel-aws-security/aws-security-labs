# VPC Lab — Subnet Isolation Steps

----------------------------------
## 🔹 BASELINE — Confirm No Communication Rule
----------------------------------

Setup:
- Public EC2 instance
- Private EC2 instance
- Same VPC

----------------------------------
## 🔹 Step 1: Try Connection (Before Allowing Access)
----------------------------------

From public EC2:

ssh private-ec2-ip

OR

curl http://private-ip

Result:
- Fails ❌

----------------------------------
## 🔹 Step 2: Confirm Security Group Rules
----------------------------------

Private EC2 SG:
- No inbound rule from public EC2

----------------------------------
## 🔹 BREAK — Remove Access Rule
----------------------------------

- Ensure NO inbound rule exists for:
  - SSH (22)
  - HTTP (80)
  - from public EC2

----------------------------------
## 🔹 Step 3: Re-Test Communication
----------------------------------

- Public EC2 → Private EC2 attempt

Result:
- Connection failed ❌

----------------------------------
## 🔹 Step 4: Confirm Root Cause
----------------------------------

Check:
- Instances running ✅
- Same VPC ✅
- No SG rule ❌

👉 Root cause = missing explicit permission
