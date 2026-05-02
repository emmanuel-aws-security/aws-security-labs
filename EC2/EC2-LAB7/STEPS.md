# EC2 Debug Lab — Case 2 Steps

----------------------------------
## 🔹 PART A — Security Group Block
----------------------------------

### Step 1: Confirm Working State
- curl http://localhost → works
- browser (public IP) → works

### Step 2: Break It (AWS Layer)
- Remove HTTP (port 80) from Security Group

### Step 3: Test Failure
- curl http://localhost → doesn't work 
- browser → fails ❌

### Step 4: Diagnose
- Service is running
- Local works
- External fails → network issue

### Step 5: Fix
- Re-add port 80 to Security Group

### Step 6: Verify
- browser works again ✅

----------------------------------
## 🔹 PART B — Port Not Listening
----------------------------------

### Step 1: Confirm Working State
- Site works normally

### Step 2: Break It (Service Layer)
- Stop nginx:
  sudo systemctl stop nginx

### Step 3: Test Failure
- curl localhost → fails ❌
- browser → fails ❌

### Step 4: Diagnose
- Check port:
  sudo ss -tulnp | grep :80

- No output → nothing listening

### Step 5: Fix
- Start nginx:
  sudo systemctl start nginx

### Step 6: Verify
- curl + browser → works ✅

----------------------------------
## 🔹 PART C — UFW Firewall Block
----------------------------------

### Step 1: Confirm Working State
- Site working

### Step 2: Break It (OS Firewall)
- Enable UFW:
  sudo ufw enable

- Deny port 80 (or don’t allow it)

### Step 3: Test Failure
- curl localhost → works ✅
- browser → fails ❌

### Step 4: Diagnose
- Check firewall:
  sudo ufw status

- Port 80 not allowed

### Step 5: Fix
- Allow HTTP:
  sudo ufw allow 80

### Step 6: Verify
- browser works again ✅
