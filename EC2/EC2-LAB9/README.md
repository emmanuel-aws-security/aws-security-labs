# EC2 Debug Lab — Case 5: App Crashes (Logs Investigation)

## 🎯 Objective
To identify and fix application failures using logs, process inspection, and port analysis.

## 🧪 Scenario
The web server or application is not starting or keeps crashing without clear external signs.

## ☁️ Environment
- EC2 (Ubuntu)
- nginx web server

## 🔍 Focus
- System logs (journalctl)
- Application logs (error.log)
- Port usage conflicts (lsof)

## 🧠 Key Idea
When a service fails silently, logs and process inspection are the only way to find the root cause.
