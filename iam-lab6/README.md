# IAM Lab 6 — Policy Conflicts (Explicit Deny vs Allow)

## 🎯 Objective
To understand how AWS resolves conflicts between IAM policies when both Allow and Deny rules exist.

## 🧪 Scenario
An IAM user is given:
- One policy that allows S3 access
- One policy that explicitly denies S3 access

The behavior is observed when both policies apply at the same time.

## ☁️ AWS Services Used
- IAM
- S3

## 🔍 Focus
- Policy evaluation order
- Explicit deny behavior
- Conflict resolution in IAM

## 🧠 Key Idea
In AWS IAM, explicit deny always overrides any allow permission.
