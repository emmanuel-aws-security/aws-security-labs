# EC2 Debug Lab — Case 4 Learnings

## 🔴 Core Issue
Incorrect file ownership and permissions prevented nginx from reading web files.

## 🧠 Key Insight
A running server does not guarantee access if the application lacks permission to read required files.

## 🔍 What Happened
- Files were owned by root
- Permissions restricted access
- nginx (running as www-data) could not read them

## ⚠️ Silent Failure
Unlike service crashes, permission issues may not immediately show obvious errors unless logs are checked.

## 🔧 Fix Applied
- Restored correct ownership (www-data)
- Set proper read/execute permissions

## 🧾 Final Conclusion
OS-level permissions are a critical layer of application availability and must be correctly configured.
