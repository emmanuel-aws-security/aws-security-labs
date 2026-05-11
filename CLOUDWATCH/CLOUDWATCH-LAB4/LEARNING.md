# CloudWatch + CloudTrail Learnings

## 🔴 Core Concept
CloudTrail and CloudWatch serve different but complementary roles in AWS security.

## 🧠 What I Learned

### CloudTrail (Audit Layer)
- records all API activity
- shows who did what
- used for investigation

### CloudWatch (Monitoring Layer)
- tracks system health and metrics
- can trigger alerts
- used for real-time monitoring

## 🔍 Key Relationship

CloudTrail:
→ logs the event

CloudWatch:
→ can detect patterns or trigger alarms based on events

## ⚠️ Security Example

Root account usage is a high-risk event because:
- it bypasses IAM controls
- has full account access
- should be monitored closely

## 🧾 Final Conclusion
CloudTrail provides forensic history, while CloudWatch provides monitoring and alerting capability.
