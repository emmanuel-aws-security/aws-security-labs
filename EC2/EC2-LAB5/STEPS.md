# EC2 Lab 7 — Steps

## Step 1: Connect to EC2
- SSH into the instance

## Step 2: Check Authentication Logs
- Ran:
  sudo cat /var/log/auth.log

- Observed:
  - SSH login attempts
  - Successful logins
  - Failed login attempts

## Step 3: Filter Login Activity (optional)
- Ran:
  sudo grep "Accepted" /var/log/auth.log

## Step 4: Check Command History
- Ran:
  history

- Observed:
  - Commands previously executed on the server

## Step 5: Analyze Findings
- Identified:
  - login times
  - source of access (IP if visible)
  - actions performed after login
