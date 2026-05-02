# EC2 Debug Lab — Case 4 Steps

----------------------------------
## 🔹 BASELINE — Confirm Working
----------------------------------

- curl http://localhost → works
- browser → works

----------------------------------
## 🔹 BREAK IT — Permission Issue
----------------------------------

### Step 1: Change ownership incorrectly
sudo chown -R root:root /var/www/html

### Step 2: Restrict permissions
sudo chmod -R 700 /var/www/html

----------------------------------
## 🔹 TEST FAILURE
----------------------------------

- curl http://localhost → may fail ❌
- browser → may show error ❌

----------------------------------
## 🔹 INVESTIGATE
----------------------------------

### Check ownership
ls -l /var/www/html

### Check logs (important)
sudo tail -f /var/log/nginx/error.log

👉 You may see:
- permission denied
- cannot open file

----------------------------------
## 🔹 FIX
----------------------------------

### Restore ownership
sudo chown -R www-data:www-data /var/www/html

### Restore permissions
sudo chmod -R 755 /var/www/html

----------------------------------
## 🔹 VERIFY
----------------------------------

- curl http://localhost → works ✅
- browser → works ✅
