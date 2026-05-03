# VPC Lab — NAT Gateway (Private Subnet Internet Access)

## 🎯 Objective
To enable internet access for a private EC2 instance without exposing it to the internet.

## 🧪 Scenario
A private EC2 instance needs to access the internet (for updates, downloads) but must not be reachable from outside.

## ☁️ AWS Services Used
- VPC
- Subnets (public + private)
- NAT Gateway
- Route Tables
- EC2

## 🔍 Focus
- Outbound-only internet access
- Secure architecture design
- Private subnet behavior

## 🧠 Key Idea
Private instances should not be publicly exposed but still need controlled outbound internet access. NAT Gateway enables this.
