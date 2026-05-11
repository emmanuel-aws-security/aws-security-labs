# EC2 Security & Debugging Lab

## 🎯 Objective
Deploy and troubleshoot EC2 instances while simulating real failure scenarios.

## 🧪 What I Built
- EC2 instance with web server (nginx)
- SSH access using key pairs
- Security groups controlling access

## 🔥 What I Tested
- Service crashes (stopping nginx)
- Port issues (80 blocked)
- Network failures (security group misconfig)
- Permission and log-based debugging

## 🧠 Debugging Flow Used
1. Check service status
2. Test local access (curl localhost)
3. Check port usage
4. Check security group rules
5. Analyze logs

## ⚠️ Security Insight
Most “server down” issues are not crashes — they are misconfigurations in network or permissions.
