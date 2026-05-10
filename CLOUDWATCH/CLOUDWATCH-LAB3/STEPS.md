# CloudWatch Logs Lab — Steps

----------------------------------
## 🔹 Step 1: Generate Logs on EC2
----------------------------------

SSH into EC2 and generate activity:

logger "CLOUDWATCH_PROOF_TEST_12345"

----------------------------------
## 🔹 Step 2: Open CloudWatch Logs
----------------------------------

Go to:
CloudWatch → Logs → Log Groups

----------------------------------
## 🔹 Step 3: Find Log Group
----------------------------------

Look for:
- /aws/ec2/*
OR
- custom log group (if configured)

----------------------------------
## 🔹 Step 4: Open Log Stream
----------------------------------

Inside log group:
- select latest log stream
- view real-time system logs

----------------------------------
## 🔹 Step 5: Observe Log Entries
----------------------------------

Check for:
- service start/stop events
- errors
- warnings
- application output

----------------------------------
## 🔹 Step 6: Compare with Local Logs
----------------------------------

On EC2:

journalctl -u amazon-cloudwatch-agent -n 50

OR

tail -f /var/log/syslog

----------------------------------
## 🔹 Step 7: Understand Centralized Logging
----------------------------------

Logs are:
- collected from EC2
- sent to CloudWatch Logs
- accessible centrally in AWS console
