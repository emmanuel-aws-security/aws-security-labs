# CloudTrail Audit & Investigation Lab

## 🎯 Lab Goal

This lab focused on understanding how AWS account activity can be tracked and investigated using CloudTrail.

The objective was to learn how actions performed inside AWS are recorded, how events can be traced back to specific users, and how audit logs support security investigations.

---

## 🧪 Environment Setup

In this lab I configured and tested:

- CloudTrail trail creation
- S3 integration for log storage
- Management event tracking
- AWS account activity monitoring

The environment was designed to capture and review actions performed inside the AWS account.

---

## 🔥 Investigation Scenarios Tested

I intentionally generated and reviewed different AWS activities, including:

- IAM user actions
- Creating and deleting S3 resources
- Event filtering by user identity
- Event filtering by event name
- Reviewing account activity through CloudTrail logs

These tests helped demonstrate how AWS actions can be traced and investigated through audit records.

---

## 🔍 Investigation Workflow

During testing, I practiced identifying:

1. Which user performed an action
2. What action was performed
3. When the action occurred
4. Which AWS service was affected
5. How to filter events for faster investigation

This helped build a clearer understanding of how CloudTrail supports visibility and accountability inside AWS environments.

---

## 🧠 Key Technical Learnings

This lab reinforced several important cloud security concepts:

- AWS actions are recorded as events inside CloudTrail
- CloudTrail helps track user and service activity across AWS resources
- Event filtering improves investigation speed during troubleshooting
- Audit logging is important for accountability and incident analysis
- CloudTrail provides visibility into changes happening inside an AWS account

The lab also improved my understanding of how AWS environments can be monitored from an audit and investigation perspective.

---

## ⚠️ Real-World Security Insight

Without audit logging, it becomes difficult to determine:
- who performed an action
- what was changed
- when the change occurred
- whether activity was authorized

This lab focused on understanding how CloudTrail helps maintain visibility and traceability during operational issues and security investigations.
