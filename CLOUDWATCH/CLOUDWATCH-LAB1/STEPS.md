# CloudWatch Lab — Steps

----------------------------------
## 🔹 Step 1: Launch EC2 Instance
----------------------------------

- Launch EC2
- Ensure instance is running

----------------------------------
## 🔹 Step 2: Open CloudWatch Metrics
----------------------------------

Go to:
CloudWatch → Metrics → EC2

Review:
- CPUUtilization
- StatusCheckFailed

----------------------------------
## 🔹 Step 3: Inspect Instance Health
----------------------------------

Go to:
EC2 → Instances

Check:
- Instance State
- Status Checks

Result:
- 2/2 checks passed ✅

----------------------------------
## 🔹 Step 4: Generate CPU Activity
----------------------------------

Inside EC2 run:

yes > /dev/null

This artificially increases CPU usage.

----------------------------------
## 🔹 Step 5: Observe CPU Spike
----------------------------------

Return to:
CloudWatch → CPUUtilization

Observe:
- increased CPU usage

----------------------------------
## 🔹 Step 6: Stop CPU Stress Test
----------------------------------

Inside EC2:

CTRL + C

OR

pkill yes

----------------------------------
## 🔹 Step 7: Create CloudWatch Alarm
----------------------------------

Create alarm for:
- CPUUtilization

Condition:
- CPU > 70%

----------------------------------
## 🔹 Step 8: Confirm Alarm State
----------------------------------

Observe:
- OK state
OR
- ALARM state during stress test
