# EC2 Lab 4 — Public vs Private EC2 Instances

## 🎯 Objective
To understand the difference between public and private EC2 instances and how network configuration controls accessibility.

## 🧪 Scenario
Two EC2 instances are created:
- One in a public subnet (accessible from the internet)
- One in a private subnet (not accessible directly from the internet)

## ☁️ AWS Services Used
- EC2
- VPC (basic understanding)
- Security Groups

## 🔍 Focus
- Public vs private subnet concept
- Network isolation
- Controlled access to resources

## ⚠️ Security Insight
Private instances should not be directly exposed to the internet (e.g., databases).

## 🧠 Key Idea
Only public instances should have direct internet access. Private instances must remain isolated.
