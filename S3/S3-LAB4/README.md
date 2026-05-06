# S3 Lab — IAM vs Bucket Policy

## 🎯 Objective
To understand how IAM policies and S3 bucket policies interact and how they can conflict.

## 🧪 Scenario
An IAM user has permission to access S3, but access is still denied due to a restrictive bucket policy.

## ☁️ AWS Services Used
- IAM
- S3

## 🔍 Focus
- IAM permissions (user/group level)
- Bucket policy (resource level)
- Policy conflict resolution

## 🧠 Key Idea
IAM says WHO can access, bucket policy says WHO is allowed on the resource. Both must allow access.

## ⚠️ Rule
If either IAM or bucket policy denies access → request fails.
