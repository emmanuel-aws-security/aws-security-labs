# EC2 Lab 3 — Steps

## Step 1: Create Security Group
- Created custom security group

## Step 2: Add Required Rules
- Allowed:
  - SSH (22) from my IP
  - HTTP (80) from 0.0.0.0/0

## Step 3: Attach to EC2
- Applied security group to instance

## Step 4: Verify Access
- SSH connection successful
- Web server accessible via browser

## Step 5: Introduce Misconfiguration
- Added unnecessary open ports (e.g., 21, 3306, 8080)
- Set source to 0.0.0.0/0

## Step 6: Confirm Exposure
- Instance now allows traffic on multiple unused ports
