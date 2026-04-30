# EC2 Lab 2 — SSH Exposure Risk (Open Port 22)

## 🎯 Objective
To demonstrate the security risk of exposing SSH (port 22) to the entire internet.

## 🧪 Scenario
An EC2 instance is configured with SSH access open to all IP addresses (0.0.0.0/0), making it publicly accessible.

## ☁️ AWS Services Used
- EC2
- Security Groups

## 🔍 Focus
- SSH exposure
- Security group misconfiguration
- Attack surface understanding

## ⚠️ Security Issue
Opening SSH to 0.0.0.0/0 allows anyone on the internet to attempt connection to the server.

## 🧠 Key Idea
Unrestricted SSH access increases risk of brute-force attacks and unauthorized access attempts.
