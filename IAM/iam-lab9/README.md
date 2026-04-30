# IAM Attack Simulation — S3 Data Exposure (Misconfiguration)

## 🎯 Objective
To simulate a real-world AWS data exposure caused by misconfigured S3 permissions, then detect and fix it.

## 🧪 Scenario
An S3 bucket is configured in a way that allows public access. Sensitive data becomes accessible without authentication.

## ☁️ AWS Services Used
- S3
- IAM
- IAM Policy Simulator

## 🔥 Security Issue
Improper bucket configuration exposes data publicly.

## 🧠 Key Idea
Misconfigured resource policies (like S3 bucket policies) can override expected IAM restrictions and expose data.
