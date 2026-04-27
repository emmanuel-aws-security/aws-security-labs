# IAM Lab 3 — Policy Deep Dive (Effect, Action, Resource)

## 🎯 Objective
To understand how IAM policies control access using JSON structure, and to observe the risks of overly broad permissions.

## 🧪 Scenario
This lab explores how different IAM policies affect user access by:
- Using an AWS managed policy (full access)
- Creating a custom restricted policy
- Comparing both behaviors

## ☁️ AWS Services Used
- IAM
- S3
- EC2 (for testing broad access)

## 🔍 Focus
Understanding how IAM policies work using:
- Effect (Allow or Deny)
- Action (what is allowed)
- Resource (where it applies)

## ⚠️ Security Issue
Overly broad permissions (e.g., `"Action": "*", "Resource": "*"`) give full control and create high security risk.

## 🧠 Key Idea
IAM policies define exactly what actions are allowed. If too broad, they remove all restrictions and expose the entire AWS account.
