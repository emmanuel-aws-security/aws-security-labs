# Mini Attack Scenario — Setup

----------------------------------
## 🔹 Step 1: Create Overexposed Environment
----------------------------------

- Launch EC2 in public subnet
- Ensure it has public IP
- Attach Security Group:

SSH (22) → 0.0.0.0/0

----------------------------------
## 🔹 Step 2: Confirm Exposure
----------------------------------

- SSH is accessible from anywhere
- Instance is reachable over internet

----------------------------------
## 🔹 Step 3: No Segmentation Design
----------------------------------

- No private subnet separation
- No restriction on inbound SSH
- Flat network structure
