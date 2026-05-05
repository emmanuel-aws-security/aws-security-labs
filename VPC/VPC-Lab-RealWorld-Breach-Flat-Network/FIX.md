# VPC Breach Simulation — Fix & Remediation

----------------------------------
## 🔧 Step 1: Re-Design Network
----------------------------------

Create:
- Public Subnet (web layer)
- Private Subnet (internal systems)

----------------------------------
## 🔧 Step 2: Move Resources
----------------------------------

- Web servers → Public subnet
- Internal apps / DB → Private subnet

----------------------------------
## 🔧 Step 3: Restrict Security Groups
----------------------------------

- SSH only from trusted IP
- No 0.0.0.0/0 exposure

----------------------------------
## 🔧 Step 4: Add NAT Gateway
----------------------------------

- Private subnet route:
  0.0.0.0/0 → NAT Gateway

----------------------------------
## 🔧 Step 5: Validate Fix
----------------------------------

- Public EC2 → reachable ✅
- Private EC2 → NOT reachable ❌
- Internal communication → controlled only via rules
