# S3 Lab — Bucket Policy Steps

----------------------------------
## 🔹 Step 1: Create Bucket
----------------------------------

- Create S3 bucket
- Upload test file

----------------------------------
## 🔹 Step 2: Confirm Private Access
----------------------------------

- Copy object URL
- Open in browser

Result:
- Access Denied ❌

----------------------------------
## 🔹 Step 3: Apply Public Read Policy
----------------------------------

- Go to bucket → Permissions → Bucket Policy
- Add policy allowing public read

Example:

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::YOUR-BUCKET-NAME/*"
    }
  ]
}

----------------------------------
## 🔹 Step 4: Test Access
----------------------------------

- Open object URL

Result:
- File accessible publicly ✅

----------------------------------
## 🔹 Step 5: Remove Policy
----------------------------------

- Delete bucket policy

----------------------------------
## 🔹 Step 6: Re-test Access
----------------------------------

Result:
- Access Denied again ❌
