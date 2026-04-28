# IAM Lab 5 — Learnings

## 🔴 Core Risk
Access keys are permanent credentials that can be used from anywhere.

## 💥 If a Key Leaks
If an attacker gets the key:
- They can access AWS resources remotely
- They can perform actions based on assigned permissions
- No login to AWS console is required

## ⚠️ Why Hardcoding is Dangerous
Placing access keys in:
- source code
- scripts
- public repositories

can expose them to attackers easily.

## 🧪 Learning from AWS CLI Testing

When I configured AWS CLI and tested S3 access through the terminal, I learned that IAM permissions are enforced consistently across both the AWS Console and CLI.

### Key Observations:
- CLI authentication depends on Access Key ID and Secret Access Key
- AWS verifies identity using `aws sts get-caller-identity`
- Permissions are not dependent on interface (console vs CLI)
- Read-only policies restrict write actions even when using CLI directly

### Security Insight:
Even with valid authentication, AWS strictly enforces authorization rules:
- Allowed actions succeed (e.g. `aws s3 ls`)
- Unauthorized actions fail immediately (e.g. upload or delete)

## 🔍 Key Understanding
IAM is enforced at the API level, not the interface level. Whether using console or CLI, the same permission rules apply.

## 🚫 Where Keys Should NEVER Be Stored
- GitHub repositories
- Public code
- Shared files
- Inside EC2 instances (hardcoded)

## 🧠 Better Approach
- Use IAM roles instead of access keys when possible
- Use temporary credentials

## 🧾 Final Conclusion
Access keys are powerful and dangerous if not handled securely. They should be avoided when roles can be used instead.
