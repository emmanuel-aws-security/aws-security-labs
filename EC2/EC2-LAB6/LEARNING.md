# EC2 Debug Lab — Case 1 Learnings

## 🔴 Core Issue
The web server stopped running, causing the site to become inaccessible.

## 🧠 Key Insight
A server can be fully operational while the application running on it is down.

## 🔍 Debugging Lesson
The first check in any failure scenario should be:
- Is the service running?

## ⚠️ Common Mistake
Assuming the entire server is down when only the application has failed.

## 🔧 Fix Applied
Restarted the nginx service and confirmed functionality.

## 🧾 Final Conclusion
Service availability is critical. Monitoring and verifying service status is the first step in troubleshooting.
