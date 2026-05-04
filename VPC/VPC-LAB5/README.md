# VPC Lab — Subnet Isolation (Lateral Movement Control)

## 🎯 Objective
To demonstrate that instances inside the same VPC cannot automatically communicate unless explicitly allowed.

## 🧪 Scenario
A public EC2 instance attempts to connect to a private EC2 instance but fails due to missing security group rules.

## ☁️ AWS Services Used
- VPC
- Subnets (public + private)
- Security Groups
- EC2

## 🔍 Focus
- Internal communication control
- Lateral movement prevention
- Security Group dependency

## 🧠 Key Idea
Being inside the same VPC does NOT mean instances can communicate. Access must be explicitly allowed.
