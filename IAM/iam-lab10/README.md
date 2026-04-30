# IAM Lab — Multi-Policy Root Cause Analysis

## 🎯 Objective
To simulate a real-world IAM environment where a user has multiple overlapping policies, then identify why access is allowed or denied using AWS IAM Policy Simulator.

## 🧪 Scenario
An IAM user is assigned multiple permissions through:
- Direct user policy
- Group policy
- Additional attached policies (allow + deny mix)

Access issues occur due to conflicting permissions.

## ☁️ AWS Services Used
- IAM
- S3
- IAM Policy Simulator

## 🔍 Focus
- Multiple policy evaluation
- Permission conflict resolution
- Root cause analysis using simulator

## 🧠 Key Idea
In real AWS environments, permissions come from multiple sources. You must trace all of them to understand the final access decision.
