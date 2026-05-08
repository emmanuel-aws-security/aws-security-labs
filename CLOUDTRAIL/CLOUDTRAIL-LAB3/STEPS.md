# CloudTrail Lab — S3 Data Events Steps

----------------------------------
## 🔹 Step 1: Create S3 Bucket
----------------------------------

- Create bucket
- Upload test file

Example:
secret-file.txt

----------------------------------
## 🔹 Step 2: Enable S3 Data Events
----------------------------------

- Open CloudTrail
- Select trail
- Edit trail settings

Enable:
- S3 Data Events

Choose:
- specific bucket
OR
- all buckets

----------------------------------
## 🔹 Step 3: Generate Object Activity
----------------------------------

Perform:
- GetObject
(read/download file)

Examples:
- open object
- download object
- use CLI

----------------------------------
## 🔹 Step 4: Investigate Activity
----------------------------------

Check:
- CloudTrail logs in S3
OR
- CloudTrail Lake

Look for:
- GetObject event
- user identity
- timestamp
- source IP

----------------------------------
## 🔹 Step 5: Confirm Visibility
----------------------------------

Result:
- Object-level access activity visible ✅
- 
