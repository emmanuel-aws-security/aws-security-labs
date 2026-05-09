# Investigation Report

## 🔍 Incident Summary
A risky S3-related action was performed inside the AWS account.

## 🔍 Investigation Process

### 1. CloudTrail Event History Reviewed
Used Event History to search for the action.

### 2. Event Filtering Applied
Filtered using:
- Event Name
-  Check manually for the IAM Username

### 3. Event Details Inspected
Identified:
- responsible IAM user
- timestamp
- source IP address

## 🧠 Findings
The action was successfully traced to a specific IAM identity through CloudTrail management events.

## ⚠️ Important Observation
Management events provided enough visibility for this investigation without requiring S3 Data Events.
