# VPC Real-World Scenario — Flat Network Disaster

## 🎯 Objective
To simulate a poorly designed VPC architecture and demonstrate how lack of segmentation leads to lateral movement risk.

## 🧪 Scenario
All workloads are deployed in a flat network with no isolation between public and internal systems.

## ☁️ AWS Services Used
- VPC
- Subnets
- EC2
- Security Groups
- Route Tables
- NAT Gateway (for fix phase)

## 🔍 Focus
- Network design flaws
- Lateral movement risk
- Security architecture failure
- Remediation strategy

## 🧠 Key Idea
If a network has no segmentation, a single compromised instance can expose the entire environment.
