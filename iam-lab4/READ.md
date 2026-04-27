# IAM Lab 4 — IAM Roles (EC2 Access to S3)

## 🎯 Objective
To understand how IAM roles allow AWS services (like EC2) to access resources securely without using access keys.

## 🧪 Scenario
An EC2 instance needs to access S3. Instead of using access keys, an IAM role is created and attached to the instance.

## ☁️ AWS Services Used
- IAM
- EC2
- S3

## 🔍 Focus
- Creating IAM roles for services
- Attaching policies to roles
- Allowing EC2 to access S3 securely

## 🧠 Key Idea
IAM roles are used by AWS services, not humans. They provide temporary credentials instead of permanent access keys.

## ⚠️ Security Advantage
Roles remove the need to store access keys inside EC2, reducing risk of credential leakage.
