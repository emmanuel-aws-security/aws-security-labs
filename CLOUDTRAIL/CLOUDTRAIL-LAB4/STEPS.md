# CloudTrail Lab — Steps

----------------------------------
## 🔹 Step 1: Generate Activity
----------------------------------

Perform multiple actions:

- Create S3 bucket
- Upload file
- Delete file
- (Optional) Create IAM user action

----------------------------------
## 🔹 Step 2: Open CloudTrail Event History
----------------------------------

Go to:
CloudTrail → Event History

----------------------------------
## 🔹 Step 3: Filter by Event Name
----------------------------------

Use filters like:

- CreateBucket
- PutObject
- DeleteObject

----------------------------------
## 🔹 Step 4: Filter by User Identity
----------------------------------

Check:
- Which IAM user performed the action

----------------------------------
## 🔹 Step 5: Open Event Details
----------------------------------

Inspect:
- Event name
- User identity
- Source IP
- Time
- Request parameters

----------------------------------
## 🔹 Step 6: Cross-check in S3 Logs (if needed)
----------------------------------

If event is missing or incomplete:
- Open CloudTrail S3 log bucket
- Search same event there

----------------------------------
## 🔹 Step 7: Confirm Full Traceability
----------------------------------

Ensure every action can be traced to:
- user
- time
- resource
