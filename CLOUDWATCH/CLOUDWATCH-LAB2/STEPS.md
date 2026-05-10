# CloudWatch Alarm Lab — Steps

----------------------------------
## 🔹 Step 1: Open CloudWatch
----------------------------------

Go to:
CloudWatch → Alarms

----------------------------------
## 🔹 Step 2: Create CPU Alarm
----------------------------------

Select metric:
EC2 → Per-Instance Metrics → CPUUtilization

Condition:
- CPU > 70%

Evaluation:
- consecutive monitoring periods

----------------------------------
## 🔹 Step 3: Name Alarm
----------------------------------

Example:
High-CPU-Alarm

Create alarm.

----------------------------------
## 🔹 Step 4: Trigger High CPU Usage
----------------------------------

Inside EC2 run:
sudo apt update
sudo apt install stress -y
stress --cpu 8

its better than yes > /dev/null
because we want to stress it above the 70 mark

This increases CPU usage artificially.

----------------------------------
## 🔹 Step 5: Observe Alarm State
----------------------------------

Check:
CloudWatch → Alarms

Observe:
- OK
- ALARM

----------------------------------
## 🔹 Step 6: Stop Stress Test
----------------------------------

Inside EC2:

CTRL + C

OR

pkill yes

----------------------------------
## 🔹 Step 7: Create Status Check Alarm
----------------------------------

Create another alarm for:
StatusCheckFailed

Purpose:
Detect unhealthy EC2 state.

----------------------------------
## 🔹 Step 8: Review Alarm Purpose
----------------------------------

CPU Alarm:
- performance issue detection

Status Check Alarm:
- infrastructure/system health detection
