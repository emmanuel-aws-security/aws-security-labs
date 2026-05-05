# VPC Breach Simulation — Steps

----------------------------------
## 🔹 PHASE 1 — Weak Design (Flat Network)
----------------------------------

Setup:
- All EC2 instances placed in ONE subnet
- All instances have public IPs
- Security Groups allow broad access (0.0.0.0/0)
- No private subnet exists

----------------------------------
## 🔹 Step 1: Confirm Exposure
----------------------------------

- All instances reachable via internet
- SSH open globally

----------------------------------
## 🔹 PHASE 2 — Attack Thinking
----------------------------------

If attacker gains access to ONE instance:

- Scan internal IP range
- Identify other running instances
- Attempt SSH or service access to them

----------------------------------
## 🔥 Risk Outcome
----------------------------------

- No segmentation
- No isolation between workloads
- Entire network becomes reachable from one entry point
