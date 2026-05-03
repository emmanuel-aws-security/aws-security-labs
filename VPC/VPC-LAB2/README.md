# VPC Lab — Route Table Deep Dive

## 🎯 Objective
To understand how route tables control internet access and to prove that removing the Internet Gateway route breaks connectivity.

## 🧪 Scenario
A public EC2 instance initially has internet access. After modifying the route table, the instance loses connectivity.

## ☁️ AWS Services Used
- VPC
- Route Tables
- Internet Gateway (IGW)
- EC2

## 🔍 Focus
- Route table behavior
- Default route (0.0.0.0/0)
- Impact of misconfiguration

## 🧠 Key Idea
Internet access in AWS depends entirely on routing. Removing the route to the Internet Gateway immediately cuts off connectivity.
