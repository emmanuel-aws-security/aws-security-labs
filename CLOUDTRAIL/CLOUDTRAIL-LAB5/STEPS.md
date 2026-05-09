# Incident Investigation — Steps

----------------------------------
## 🔹 Step 1: Create IAM User
----------------------------------

- Create IAM user
- Grant limited S3 permissions

----------------------------------
## 🔹 Step 2: Generate Activity
----------------------------------

Using the IAM user:

Perform ONE risky action:
- CreateBucket
OR
- DeleteBucket
OR
- Modify bucket public access settings

----------------------------------
## 🔹 Step 3: Open CloudTrail
----------------------------------

Go to:
CloudTrail → Event History

----------------------------------
## 🔹 Step 4: Search for Event
----------------------------------

Filter by:
- Event Name
OR
- Username

Examples:
- CreateBucket
- DeleteBucket
- PutBucketPolicy

----------------------------------
## 🔹 Step 5: Open Event Details
----------------------------------

Identify:
- IAM user
- Event time
- Source IP address
- AWS service
- Event source

----------------------------------
## 🔹 Step 6: Confirm Traceability
----------------------------------

Result:
- Suspicious action successfully traced ✅
