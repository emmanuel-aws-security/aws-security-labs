# Detection Notes — CloudTrail Incident Investigation

## 🎯 Goal
Understand how suspicious AWS activity can be detected using CloudTrail management events.

----------------------------------
## 🔍 What Was Detected
----------------------------------

The following risky S3-related activity was identified:

- Bucket creation
- Bucket deletion
- Bucket policy modification
- Public access configuration changes

These actions were visible through CloudTrail management events.

----------------------------------
## 🔍 Detection Method
----------------------------------

Detection was performed using:

CloudTrail → Event History

Filters used:
- Event Name
- Username
- Time range

----------------------------------
## 🔍 Indicators of Suspicious Activity
----------------------------------

Examples of suspicious indicators:

### 1. Unexpected Bucket Deletion
Event:
DeleteBucket

Risk:
- potential data destruction
- accidental deletion
- malicious insider activity

### 2. Public Access Changes
Event:
PutBucketPolicy
PutBucketPublicAccessBlock

Risk:
- accidental exposure
- public data leak

### 3. Unknown IAM User Activity
Risk:
- compromised credentials
- unauthorized usage

### 4. Unrecognized Source IP
Risk:
- access from unexpected location
- possible attacker infrastructure

----------------------------------
## 🔍 Important Investigation Fields
----------------------------------

During investigation, these fields were reviewed:

- IAM user identity
- Event name
- Source IP address
- Timestamp
- AWS region

----------------------------------
## 🧠 Detection Insight
----------------------------------

CloudTrail management events provide visibility into important AWS account changes and administrative actions.

This allows security teams to:
- identify risky behavior
- trace account activity
- investigate incidents

----------------------------------
## ⚠️ Important Limitation
----------------------------------

This lab focused ONLY on:
- Management Events

NOT:
- S3 object-level Data Events

Meaning:
- bucket-level administrative activity was visible
- object access visibility was limited

----------------------------------
## 🧾 Final Conclusion
----------------------------------

CloudTrail management events are critical for detecting:
- risky account activity
- configuration changes
- suspicious administrative actions

Detection depends on:
- proper logging
- proper filtering
- correct investigation workflow
