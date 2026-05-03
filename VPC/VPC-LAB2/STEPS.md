# VPC Lab — Route Table Deep Dive Steps

----------------------------------
## 🔹 BASELINE — Confirm Working
----------------------------------

- EC2 in public subnet
- Route table has:
  0.0.0.0/0 → IGW

Test:
- curl http://google.com → works ✅

----------------------------------
## 🔹 Step 1: Inspect Route Table
----------------------------------

- Open route table
- Identify:
  - Local route (VPC CIDR)
  - Internet route:
    0.0.0.0/0 → IGW

----------------------------------
## 🔹 BREAK — Remove Internet Route
----------------------------------

- Delete:
  0.0.0.0/0 → IGW

----------------------------------
## 🔹 Step 2: Test Connectivity
----------------------------------

Run:
ssh into server

Result:
- fails ❌

Browser:
- site unreachable ❌

----------------------------------
## 🔹 Step 3: Confirm Root Cause
----------------------------------

- EC2 still running ✅
- nginx still running (if installed) ✅
- Only routing changed ❌

👉 Root cause = no route to internet

----------------------------------
## 🔹 FIX — Restore Route
----------------------------------

- Add back:
  0.0.0.0/0 → IGW

----------------------------------
## 🔹 Step 4: Re-test
----------------------------------

ssh into the server→ works ✅
