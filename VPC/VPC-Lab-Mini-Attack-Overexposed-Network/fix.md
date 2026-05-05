# Attack Scenario — Thinking Like an Attacker

## 🔴 Entry Point
- SSH open to world (0.0.0.0/0)

## 🧠 What attacker does
- Scan public IP ranges
- Attempt brute-force SSH login
- Identify weak credentials or misconfigurations

## 💥 Impact if compromised
- Full server access
- File system access
- Credential theft
- Lateral movement to other services (if exist)

## ⚠️ Core Risk
There is no network boundary preventing entry.
