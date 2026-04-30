# IAM Lab 1 — Learnings

## 🧠 IAM Structure Understanding
IAM access works in a hierarchy:
- User = identity (who you are)
- Group = collection of users
- Policy = rules that define permissions

## 🔑 What I Learned
- Users do not usually get permissions directly
- Groups make permission management easier and scalable
- Policies define what actions are allowed or denied

## ⚠️ Root Account Risk
The root account should never be used for daily tasks because:
- It has full unrestricted access to the entire AWS account
- It cannot be limited by IAM policies
- If compromised, the entire AWS account is at risk

  ## 🧪 Learning from Permission Testing

While testing S3 access, I attempted actions that were NOT included in the policy (such as upload, delete, and bucket creation).

These actions were explicitly denied by AWS, which confirmed that:
- IAM enforces both allowed and denied actions strictly
- Missing permissions automatically result in denial
- Read-only access does not allow any modification operations

## 🔍 Key Insight
IAM is not just about what is permitted — it is equally about what is restricted. Any action not explicitly allowed by the policy is denied by default.

## 🧾 Final Understanding
IAM is designed so that access is structured and controlled, not randomly assigned to individual users.
