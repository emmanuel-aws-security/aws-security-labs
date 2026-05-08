# CloudTrail Lab — Learnings

## 🔴 Core Concept
CloudTrail is not meant to be used by scrolling — it is meant to be used by filtering and querying.

## 🧠 What I Learned

### 1. Event History is for quick checks
- Good for fast visibility
- Not complete for deep investigations

### 2. Filtering is the real skill
- Event name filtering
- IAM user filtering did not show 
- Resource-based filtering

### 3. Deep logs may exist elsewhere
- S3 CloudTrail logs contain full records
- Event History may not show everything

## 🔍 Key Insight
Real cloud security work is about narrowing down events, not searching manually.

## ⚠️ Important Lesson
If you cannot filter properly, you cannot investigate incidents in real environments.

NOTE:
After the lab test i found out you cannot filet based on username but you can filter in event history based on event id ,event name,
resource name , resource type , aws access key , read only and event source.

## 🧾 Final Conclusion
Filtering is the core skill for CloudTrail-based investigation.
