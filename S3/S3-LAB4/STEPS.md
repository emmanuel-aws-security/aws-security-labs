# S3 Lab — IAM vs Bucket Policy Steps

----------------------------------
## 🔹 Step 1: Setup IAM User
----------------------------------

- Create IAM user
- Attach policy:
  - AmazonS3FullAccess (or limited S3 access)

----------------------------------
## 🔹 Step 2: Create S3 Bucket
----------------------------------

- Upload test file

----------------------------------
## 🔹 Step 3: Confirm IAM Access Works
----------------------------------

- Use IAM user credentials
- Try accessing bucket

----------------------------------
## 🔹 Step 4: Add Restrictive Bucket Policy
----------------------------------

- Deny access OR limit access to another user

Example:

{
  "Effect": "Deny",
  "Principal": "*",
  "Action": "s3:GetObject",
  "Resource": "arn:aws:s3:::YOUR-BUCKET/*"
}

----------------------------------
## 🔹 Step 5: Test Access Again
----------------------------------

Result:
- Access denied ❌

----------------------------------
## 🔹 Step 6: Remove Bucket Policy
----------------------------------

- Delete or adjust policy

----------------------------------
## 🔹 Step 7: Retest Access
----------------------------------

Result:
- Access works again ✅
