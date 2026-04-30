# EC2 Lab 3 — Security Groups Deep Dive (Firewall Misconfiguration)

## 🎯 Objective
To understand how security groups control access to EC2 instances and how overly permissive rules increase attack surface.

## 🧪 Scenario
A custom security group is created to allow required access (SSH and HTTP), then misconfigured by adding unnecessary open ports.

## ☁️ AWS Services Used
- EC2
- Security Groups

## 🔍 Focus
- Firewall rule configuration
- Required vs unnecessary access
- Attack surface expansion

## ⚠️ Security Issue
Opening ports that are not required exposes the instance to unnecessary risk.

## 🧠 Key Idea
Security groups act as firewalls. Only required ports should be open.
