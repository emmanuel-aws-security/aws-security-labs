# EC2 Lab 1 — Steps

## Step 1: Launch EC2 Instance
- Selected Ubuntu AMI
- Created or selected key pair
- Allowed:
  - SSH (port 22)
  - HTTP (port 80)

## Step 2: Connect via SSH
- Used private key (.pem file)
- Connected from local machine using SSH

## Step 3: Install Web Server
- Ran:
  sudo apt update
  sudo apt install nginx -y

## Step 4: Verify Service Locally
- Ran:
  curl http://localhost
- Confirmed nginx response

## Step 5: Verify External Access
- Opened in browser:
  http://<EC2-PUBLIC-IP>
- Confirmed web server is reachable
