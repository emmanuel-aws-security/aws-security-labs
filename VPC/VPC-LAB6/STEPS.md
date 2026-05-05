# VPC Lab — Flow Logs Steps

----------------------------------
## 🔹 Step 1: Enable Flow Logs
----------------------------------

- Go to VPC console
- Select VPC
- Enable Flow Logs
- Destination:
  - CloudWatch Logs (or S3)

----------------------------------
## 🔹 Step 2: Generate Traffic
----------------------------------

From EC2 instances:
- SSH attempts
- curl requests
- blocked connections

----------------------------------
## 🔹 Step 3: View Logs
----------------------------------

In CloudWatch:
- Open Flow Log group
- Inspect entries

----------------------------------
## 🔹 Step 4: Identify Traffic Types
----------------------------------

Look for:
- ACCEPT → allowed traffic
- REJECT → blocked traffic

----------------------------------
## 🔹 Step 5: Break & Confirm
----------------------------------

- Block traffic (Security Group or NACL)
- Retry connection
- Confirm REJECT appears in logs
