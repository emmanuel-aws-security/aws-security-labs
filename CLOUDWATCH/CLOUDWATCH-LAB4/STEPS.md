# CloudTrail + CloudWatch Integration Steps

----------------------------------
## 🔹 Step 1: Ensure CloudTrail is Enabled
----------------------------------

- CloudTrail trail active
- Management events enabled

----------------------------------
## 🔹 Step 2: Perform a Sensitive Action
----------------------------------

Examples:
- Sign in as root (if available)
- Create S3 bucket
- Delete resource
- Change IAM settings

----------------------------------
## 🔹 Step 3: View CloudTrail Event
----------------------------------

Go to:
CloudTrail → Event History

Check:
- event name
- user identity
- source IP
- timestamp

----------------------------------
## 🔹 Step 4: Understand Detection Flow
----------------------------------

CloudTrail captures:
- raw AWS activity logs

CloudWatch can:
- monitor metrics/log patterns
- trigger alarms based on behavior (conceptually)

----------------------------------
## 🔹 Step 5: Example Security Signal

Root user used → high-risk event

Detection idea:
- unusual identity usage
- sensitive API call

----------------------------------
## 🔹 Step 6: Awareness Check
----------------------------------

Understand:
- CloudTrail = recording layer
- CloudWatch = monitoring + alert layer
