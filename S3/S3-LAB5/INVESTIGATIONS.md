# S3 Exposure — Investigation

## 🔍 Step 1: Check Bucket Settings
- Verify public access settings
- Confirm object-level permissions

## 🔍 Step 2: Check Bucket Policy
- Look for:
  "Principal": "*"
  "s3:GetObject"

## 🔍 Step 3: Identify Root Cause
- Public access enabled
- No access restriction applied

## 🧠 Finding
Data is exposed due to misconfigured permissions at bucket level.
