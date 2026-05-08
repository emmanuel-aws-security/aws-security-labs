# CloudTrail Lab — Steps

----------------------------------
## 🔹 Step 1: Create S3 Bucket
----------------------------------

- Create test bucket
- Upload sample file

----------------------------------
## 🔹 Step 2: Perform Action
----------------------------------

- Delete uploaded object

----------------------------------
## 🔹 Step 3: Open CloudTrail
----------------------------------

- Go to:
CloudTrail → Event History

----------------------------------
## 🔹 Step 4: Search Events
----------------------------------

Filter using:
- Event Name
OR
- Resource Name

Example:
PutObject

----------------------------------
## 🔹 Step 5: Investigate Event
----------------------------------

Identify:
- Event name
- IAM user
- Timestamp
- Source IP address
- AWS service involved

----------------------------------
## 🔹 Step 6: Confirm Investigation
----------------------------------

Result:
- Deletion activity traced successfully ✅
- the data event was visbile but it was in the s3 logs the data  event didnt appear in the event history
