# EC2 Breach Simulation — Investigation

## 🔍 Step 1: Check SSH Access Logs
sudo cat /var/log/auth.log

- Look for:
  - successful logins
  - unknown IP addresses
  - repeated failed attempts

## 🔍 Step 2: Check Running Activity
ps aux

- Identify suspicious processes

## 🔍 Step 3: Check File System
ls -la

- Look for sensitive files:
  - creds.txt
  - config files
  - hidden files

## 🔍 Step 4: Check Web Server Logs
sudo tail -f /var/log/nginx/access.log

- Identify unusual access patterns

## 🧠 Findings Summary
- Instance exposed via SSH
- Sensitive file present on system
- No restrictions on access
