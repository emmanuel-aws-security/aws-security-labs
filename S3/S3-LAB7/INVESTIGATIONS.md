# Investigation — Finding the Root Cause

## 🔍 Step 1: Check Public Access Settings
- Block Public Access disabled

## 🔍 Step 2: Check Bucket Policy
- Look for:
  "Principal": "*"
  "Effect": "Allow"
  "Action": "s3:GetObject"

## 🔍 Step 3: Check Object Permissions
- Object marked as public

## 🧠 Root Cause
Misconfigured access control allowed unrestricted public access.

## ⚠️ Key Finding
No authentication required to access sensitive data.
