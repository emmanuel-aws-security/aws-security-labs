# VPC Lab — Security Groups vs NACL (Layered Control)

## 🎯 Objective
To demonstrate how Security Groups and Network ACLs work together and how explicit deny at the NACL level overrides allowed traffic.

## 🧪 Scenario
Traffic is allowed at the instance level (Security Group) but blocked at the subnet level (NACL), causing unexpected connection failure.

## ☁️ AWS Services Used
- VPC
- Subnets
- Security Groups
- Network ACLs (NACL)
- EC2

## 🔍 Focus
- Difference between SG and NACL
- Layered security enforcement
- Deny vs Allow behavior

## 🧠 Key Idea
Security Groups allow traffic, but NACLs can still block it. Both layers must permit traffic for communication to succeed.
