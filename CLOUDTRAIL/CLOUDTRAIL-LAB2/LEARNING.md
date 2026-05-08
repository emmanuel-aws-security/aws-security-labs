# CloudTrail Lab — Learnings

## 🔴 Core Concept
CloudTrail provides visibility into AWS account activity.

## 🧠 What I Learned
CloudTrail events contain:
- who performed the action
- what action occurred
- when it happened
- where it came from
- to check s3 object visbility you need cloud lake
  
## 🔍 Investigation Insight
Even destructive actions like object deletion can be traced.
Event History ≠ full S3 object(e.g putobject,deleteobject) visibility

## ⚠️ Security Importance
Without logging:
- malicious activity may go unnoticed
- investigations become difficult

## 🧾 Final Conclusion
CloudTrail is critical for accountability and incident investigation in AWS.
