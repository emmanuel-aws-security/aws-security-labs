# EC2 Debug Lab — Case 5 Learnings

## 🔴 Core Problem Types in App Failures

### 1. Missing File / Config Issue
- App cannot find required files
- Causes startup or runtime failure

### 2. Port Conflict
- Another process is using required port
- Service cannot bind to port 80

### 3. System Error
- Service fails internally
- Requires restart or config correction



## 🔍 Key Tools

### journalctl
- Shows system-level service logs
- Used for startup and crash analysis

### error.log
- Shows application-level errors
- Useful for file/path issues

### lsof -i :80
- Shows which process is using a port
- Critical for debugging port conflicts

## 🧠 Core Insight
Most “random crashes” are not random:
They are caused by file, port, permission, or config issues.

## ⚠️ Mistake to avoid
Restarting blindly without checking logs.
