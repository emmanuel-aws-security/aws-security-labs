# VPC Lab 1 — Steps

----------------------------------
## 🔹 Step 1: Create VPC
----------------------------------
- Created custom VPC
- CIDR block: 10.0.0.0/16

----------------------------------
## 🔹 Step 2: Create Subnets
----------------------------------
- Public Subnet:
  - CIDR: 10.0.1.0/24

- Private Subnet:
  - CIDR: 10.0.2.0/24

----------------------------------
## 🔹 Step 3: Attach Internet Gateway
----------------------------------
- Created Internet Gateway (IGW)
- Attached IGW to VPC

----------------------------------
## 🔹 Step 4: Create Route Table (Public)
----------------------------------
- Created route table
- Added route:
  - 0.0.0.0/0 → Internet Gateway

----------------------------------
## 🔹 Step 5: Associate Public Subnet
----------------------------------
- Associated public subnet with this route table

----------------------------------
## 🔹 Step 6: Launch EC2 Instances (for testing)
----------------------------------
- Launched EC2 in:
  - Public subnet
  - Private subnet

----------------------------------
## 🔹 Step 7: Test Internet Access
----------------------------------

### Public EC2:
- SSH works
- curl google.com → works

### Private EC2:
- No public IP
- curl google.com → fails

----------------------------------
## 🔹 Step 8: Validate Behavior
----------------------------------
- Public subnet has internet access
- Private subnet has no internet access
