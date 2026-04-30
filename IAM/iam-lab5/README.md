# IAM Lab 5 — Access Keys Risk (Credential Exposure)

## 🎯 Objective
To understand how AWS access keys work and the security risks if they are exposed.

## 🧪 Scenario
An IAM user is given an access key and uses it via AWS CLI to access resources.

## ☁️ AWS Services Used
- IAM
- S3
- AWS CLI

## 🔍 Focus
- Creating access keys
- Using them for authentication
- Understanding risks of exposure

## CLI Configuration
- Configured AWS CLI using access keys
- Verified identity using `aws sts get-caller-identity`

## S3 Access via CLI
- Listed buckets successfully using `aws s3 ls`
- Attempted upload → Access Denied (confirms read-only policy)

## ⚠️ Security Issue
Access keys are long-term credentials. If leaked, they can be used to access AWS resources without restrictions (depending on permissions).

## 🧠 Key Idea
Access keys should be protected and never stored in insecure locations.
