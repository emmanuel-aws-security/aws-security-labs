# CloudTrail Lab — Steps

----------------------------------
## 🔹 Step 1: Create S3 Bucket
----------------------------------

- Go to S3
- Create bucket for CloudTrail logs

Example:
cloudtrail-logs-lab

----------------------------------
## 🔹 Step 2: Create CloudTrail Trail
----------------------------------

- Go to CloudTrail
- Click Create Trail

Configuration:
- Trail name
- Enable for all regions ✅
- Create/use S3 bucket
- Enable logging

----------------------------------
## 🔹 Step 3: Generate Activity
----------------------------------

Perform simple AWS actions:
- Create bucket
- Upload file
- View EC2

----------------------------------
## 🔹 Step 4: Confirm Log Delivery
----------------------------------

- Open S3 bucket
- Navigate through log folders

Result:
- CloudTrail log files delivered ✅

----------------------------------
## 🔹 Step 5: Check Event History
----------------------------------

- Open CloudTrail → Event History
- Confirm events appear

Examples:
- CreateBucket
- PutObject
- DescribeInstances
