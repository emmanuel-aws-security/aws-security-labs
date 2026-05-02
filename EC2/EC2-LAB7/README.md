# EC2 Debug Lab — Case 2: Site Not Loading (Network / Port / Firewall)

## 🎯 Objective
To diagnose why a web server is not accessible externally by testing network rules, service ports, and internal firewall settings.

## 🧪 Scenario
The web server is running but cannot be accessed from the internet.

## ☁️ Environment
- EC2 (Ubuntu)
- nginx web server

## 🔍 Focus
- Security Groups (AWS layer)
- Port listening (service layer)
- UFW firewall (OS layer)

## 🧠 Key Idea
External access requires:
- service running
- port listening
- network allowing traffic
