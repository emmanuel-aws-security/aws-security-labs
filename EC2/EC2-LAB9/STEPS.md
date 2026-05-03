# EC2 Debug Lab — Case 5 Steps

----------------------------------
## 🔹 BASELINE — Confirm Working
----------------------------------

- curl http://localhost → works
- browser → works

----------------------------------
## 🔹 BREAK 1 — Service Crash
----------------------------------

### Step 1: Stop service
sudo systemctl stop nginx

### Step 2: Simulate failure
- curl http://localhost → fails ❌

### Step 3: Check logs
sudo journalctl -u nginx

👉 Look for:
- service stop messages
- startup errors

### Fix
sudo systemctl start nginx

----------------------------------
## 🔹 BREAK 2 — Missing File / Config Issue
----------------------------------

### Step 1: Break config or remove file
- delete or rename index file

### Step 2: Test
- curl localhost → fails ❌

### Step 3: Check error logs
sudo tail -f /var/log/nginx/error.log

👉 Possible output:
- file not found
- invalid path

### Fix
- restore missing file
- fix nginx config path
- reload nginx:
  sudo systemctl reload nginx

----------------------------------
## 🔹 BREAK 3 — Port Conflict
----------------------------------

### Step 1: Create conflict
- run another service on port 80 (or simulate conflict)

### Step 2: Check port usage
sudo lsof -i :80

👉 You will see:
- process ID (PID)
- service using port 80

### Step 3: Test
- nginx fails to start or bind ❌

### Fix Option 1 — Kill process
sudo kill -9 <PID>

### Fix Option 2 — Change nginx port
- edit config file
- restart nginx

----------------------------------
## 🔹 BREAK 4 — Permission Issue (Link to Case 4)

### Step 1: Restrict file access
- change ownership or permissions

### Step 2: Check logs
- nginx error.log shows:
  permission denied

### Fix
- restore ownership:
  sudo chown -R www-data:www-data /var/www/html
