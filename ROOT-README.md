# AWS Cloud Security & Incident Response Labs

## 🎯 Overview
This repository demonstrates a hands-on cloud security environment built on AWS, focusing on deployment, misconfiguration, monitoring, and incident investigation.

I simulate real-world cloud environments where systems are intentionally broken, monitored, and investigated using AWS security tools.

---

## 🧠 What I Built

- EC2 instances for application hosting
- VPC with public and private subnets
- S3 buckets with controlled exposure scenarios
- IAM users and roles with different permission models
- CloudTrail for audit logging
- CloudWatch for monitoring and alerting

---

## 🔥 What I Practiced (IMPORTANT)

I did not only deploy infrastructure — I:

- Intentionally misconfigured systems
- Simulated real failures (service crash, network blocks, permission errors)
- Tested exposure risks (open SSH, public S3 access)
- Investigated incidents using logs and metrics
- Fixed root causes using structured debugging

---

## 🧪 Core Skills Demonstrated

- Cloud infrastructure setup (AWS basics)
- Security misconfiguration awareness
- Incident investigation (CloudTrail)
- System monitoring (CloudWatch)
- Network isolation (VPC design)
- Linux troubleshooting (logs, services, permissions)

---

## 🔍 Thinking Approach

When something breaks, I follow:

1. Is the service running?
2. Is the port open?
3. Can I reach it locally?
4. Is network blocking it?
5. What do logs say?
6. Is it IAM-related?

---

## ⚠️ Key Outcome

I understand cloud systems as layered environments:
- Compute layer (EC2)
- Network layer (VPC)
- Identity layer (IAM)
- Logging layer (CloudTrail)
- Monitoring layer (CloudWatch)
- Storage layer (S3)

Failures can occur at any layer — I learned how to isolate them systematically.

---

## 📌 Projects Inside This Repo

Each folder contains:
- README (what was built)
- steps (what was done)
- learnings (what was learned)
- evidence (screenshots of results)

## Some folders contain:
-invsetigation(the structure to troubleshooting problem)
-fix (how i fix the problems)

---



## 🚀 Goal

To demonstrate practical AWS cloud security skills through hands-on deployment, monitoring, troubleshooting, and incident investigation labs.
