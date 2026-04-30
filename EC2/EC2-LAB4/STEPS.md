# EC2 Lab 4 — Steps

## Step 1: Create Two EC2 Instances
- Instance 1: Public EC2
  - Placed in public subnet
  - Auto-assign public IP enabled

- Instance 2: Private EC2
  - Placed in private subnet
  - No public IP assigned

## Step 2: Configure Security Groups
- Public instance:
  - Allow SSH (22) from my IP

- Private instance:
  - Allow SSH only from public instance (optional test setup)

## Step 3: SSH into Public Instance
- Connected successfully using key pair

## Step 4: Attempt SSH into Private Instance
- Attempted connection using private IP
- Connection failed

## Step 5: Confirm Isolation
- Verified private instance is not reachable from internet
