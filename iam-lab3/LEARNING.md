# IAM Lab 3 — Learnings

## 🧠 Policy Structure Understanding

IAM policies are written in JSON and contain:

- Effect → defines whether an action is allowed or denied
- Action → specifies what operations can be performed
- Resource → defines which resources the actions apply to

## 🔴 Over-Permissioning Risk

When using:
- "Action": "*"
- "Resource": "*"

The user gains full control over all AWS services.

## 💥 What Happens When Permissions Are Too Broad?

- User can access and modify any resource
- No restriction on critical services (IAM, EC2, S3)
- In case of compromise:
  - attacker can delete infrastructure
  - attacker can exfiltrate data
  - attacker can create backdoors

## ⚖️ Before vs After

### Before (Admin Access):
- Full control across AWS
- No restrictions

### After (Custom Policy):
- Limited to S3 read-only
- No access to other services

## 🧠 Key Security Concept
Least Privilege:
Users should only have the permissions required for their task, nothing more.

## 🧾 Final Conclusion
IAM policies are the core control mechanism in AWS. Poorly defined policies (especially overly broad ones) create major security risks.
