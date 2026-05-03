# VPC Lab — NAT Gateway Steps

----------------------------------
## 🔹 BASELINE — Confirm Private Has No Internet
----------------------------------

- EC2 in private subnet
- No NAT configured

Test:
- curl http://google.com → fails ❌

----------------------------------
## 🔹 Step 1: Create NAT Gateway
----------------------------------

- Create NAT Gateway in PUBLIC subnet
- Attach Elastic IP

----------------------------------
## 🔹 Step 2: Update Private Route Table
----------------------------------

- Edit private subnet route table
- Add:
  0.0.0.0/0 → NAT Gateway

----------------------------------
## 🔹 Step 3: Test Outbound Access
----------------------------------

From private EC2:

- curl http://google.com → works ✅
- sudo apt update → works ✅

----------------------------------
## 🔹 Step 4: Test Inbound Access (IMPORTANT)
----------------------------------

From your local machine:

- Try SSH to private EC2 → fails ❌

Reason:
- No public IP
- No IGW route

----------------------------------
## 🔹 Step 5: Validate Behavior
----------------------------------

- Outbound → allowed ✅
- Inbound → blocked ❌

👉 This is expected behavior
