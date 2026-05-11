# IAM Security Lab

## 🎯 Lab Goal

This lab focused on understanding how identity and access management controls access to AWS resources, and how misconfigured permissions can create security exposure across an entire cloud environment.

The objective was not only to create IAM resources, but to understand how permissions are evaluated, abused, and secured in practical scenarios.

---

## 🧪 Environment Setup

In this lab I configured and tested:

- IAM users and groups
- Managed IAM policies
- Least-privilege permission models
- Over-permissioned access scenarios
- IAM roles attached to EC2 instances
- Temporary credential usage through role assumption

The environment was structured to compare secure vs insecure access approaches across AWS services.

---

## 🔥 Security Scenarios Simulated

I intentionally tested multiple access-control scenarios, including:

- Access using IAM user credentials
- Access using IAM roles attached to EC2
- Permission denial troubleshooting
- Overly permissive policy behavior
- Hardcoded credential exposure risks
- Policy evaluation and permission inheritance

This helped demonstrate how small IAM mistakes can lead to excessive access inside cloud environments.

---

## 🔍 Investigation & Troubleshooting

During testing, I verified:

- Whether permissions originated from users, groups, or attached policies
- How AWS evaluates allow vs deny logic
- How role-based authentication differs from static credentials
- Why permission debugging often requires tracing multiple policy layers

I also practiced identifying root causes of access failures instead of assuming permission issues immediately.

---

## 🧠 Key Security Takeaways

This lab reinforced several important security principles:

- IAM is a foundational security layer in AWS
- Excessive permissions significantly increase attack surface
- Hardcoded credentials create long-term exposure risk
- IAM roles are safer and more scalable than embedding access keys
- Effective troubleshooting requires understanding permission inheritance and policy evaluation flow

---

## ⚠️ Real-World Security Relevance

IAM misconfigurations are one of the most common causes of cloud security incidents.

Even when infrastructure is configured correctly, excessive permissions or exposed credentials can still result in unauthorized access, privilege escalation, or data exposure.

This lab focused on understanding those risks from both operational and defensive perspectives.
